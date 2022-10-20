public class Main {

    /**
     * 2014年统考
     * 求叶节点的带权路径长度
     */

    public int sum = 0;

    public static void main(String[] args) {
        TreeNode t1 = new TreeNode(3,null,null);
        TreeNode t2 = new TreeNode(2,null,null);
        TreeNode t3 = new TreeNode(5,null,null);
        TreeNode t4 = new TreeNode(4,t1,t2);
        TreeNode t5 = new TreeNode(1,t4,t3);
        Main main = new Main();
        main.dfs(t5,0);
        System.out.println(main.sum);

    }

    void dfs(TreeNode t, int len) {

        if (t == null) return;
        if (t.left == null && t.right == null){
            sum += len* t.val;
        }
        dfs(t.left , len + 1);
        dfs(t.right , len + 1);
    }
}


class TreeNode {
    int val;
    TreeNode left;
    TreeNode right;

    TreeNode() {
    }

    TreeNode(int val) {
        this.val = val;
    }

    TreeNode(int val, TreeNode left, TreeNode right) {
        this.val = val;
        this.left = left;
        this.right = right;
    }
}
