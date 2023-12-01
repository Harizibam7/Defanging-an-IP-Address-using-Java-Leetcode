# Defanging-an-IP-Address-using-Java-Leetcode

    class Solution {
        public String defangIPaddr(String address) {
            String ip = "";
            String open = "[";
            String close = "]";
            for(int i =0;i<address.length();i++){
                if(address.charAt(i)==('.')){
                    ip+=open;
                    ip+=".";
                    ip+=close;
                }else{
                    ip+=address.charAt(i);
                }
            }
            return ip;
        }
    }
