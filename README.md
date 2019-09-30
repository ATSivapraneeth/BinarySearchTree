# BinarySearchTree

public class BST {
	protected BSTNode root;
	public void insert(int key)
	{
		if (root==null)
		{
			root=new BSTNode(key);
		}
		else
			root.insert(key);
	}
	public void inorder()
	{
		if(root==null)
			return;
		else
			root.inorder();
	}
	public boolean search(int key)
	{
		if(root ==null)
			return false;
		else
			return root.search(key);
	}
	public int tree_min(int p)
	{
		if(root == null)
			return 0;
		else
			return root.tree_min(p);
	}
	public int tree_max(int k)
	{
		if(root == null)
			return 0;
		else
			return root.tree_max(k);
	}
	public int height()
	{
		if(root == null)
			return -1;
		else
			return root.height();
	}
}
