# Gx_kj
java code

treeset can change
  TreeSet<String> myTree=new TreeSet<>(new Comparator() {
            @Override
            public int compare(Object lhs, Object rhs) {
                int left=Integer.valueOf(lhs.toString().substring(0,2));
                int right=Integer.valueOf(rhs.toString().substring(0,2));
                if(left>right)
                {
                    return 1;
                }
                if(left==right)
                {
                    return 0;
                }
                if(left<right)
                {
                    return -1;
                }
                return -1;
            }
        });
        myTree.add("01清华听");
        myTree.add("13清华听");
        myTree.add("04清华听");
        myTree.add("15清华听");
        myTree.add("15清华听");
        myTree.add("07清华听");
        myTree.add("02清华听");
        myTree.add("03清华听");

        for ( String s:myTree )
        {
            Log.e("**",s+"");
        }

