# rev-a-string
char* reverse(char *S, int len)
{
    //code here
    stack<char>s;
    for(int i=0;i<len;i++){
        char ch=S[i];
        s.push(ch);
    }
    for(int i=0;i<len;i++){
    S[i]=s.top();
    s.pop();
    
    }
    return S;
}
