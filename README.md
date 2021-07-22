### STL
所有容器迭代器失效的场景 做个笔记 以后方便回顾


### Vecotor
	reverse 若new大于原来的capacity 则 所有迭代器全部失效 因为vector自动扩张把所有的元素全部换了一个位置
	insert  若插入的元素个数(size)大于当前容量(capacity) 所有迭代器全部失效 因为vector自动扩张把所有的元素全部换了一个位置 
			否则 仅当前插入位置后面的所有迭代器全部失效(因为vector自动扩张把所有的元素全部换了一个位置)
	emplace     同上
	erase       当前节点之后的所有迭代器全部失效
	shrink_to_fit capacity发生改变 则 所有的迭代器 全部失效
	
