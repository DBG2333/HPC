# 1. 快速排序
```
vector exchange(arr,k)
{
vector_r=[]
vector_l=[]
temp=arr[k]
for(i=left,i<right,i++)
if(arr[k]>a[i]) vector_r.push_back(arr[k]);
else
vector_l.push_back(arr[k]);

return [vector_l,arr[k],vector_r]

}
void QS(arr, left, right)
{
if(len(arr)=1)return;
else
exchange(arr,right-1);

}

QS(arr,0,n-1)
```
