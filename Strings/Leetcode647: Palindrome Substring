
class Solution {
public:
//TC- O(n)
int expand( string s, int i , int j ){
        int count = 0;
//Two pointer approach
        while(i>= 0 && j < s.length() && s[i]==s[j]){
            count++;
            i--;
            j++;
        }
        return count;
    }

    int countSubstrings(string s) {
        int totalCount = 0 ;
        for(int center = 0 ; center < s.length() ; center++){
            int oddKaAns = expand(s,center, center);
            int evenKaAns = expand(s , center, center + 1);
            totalCount = oddKaAns + evenKaAns + totalCount;
            
        }
        return totalCount;
    }
};
