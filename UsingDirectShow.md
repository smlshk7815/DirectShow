## 使用步驟
1. 使用 CoInitialize 初始化 COM
2. 建立特定 ID 的實體: CoCreateInstance
3. 使用 ICreateDevEnum 的 CreateClassEnumerator
4. 使用 IEnumMoniker 指到的物件去列舉並使用 IMoniker* 指到他
5. BindToStorage
6. 使用 IPropertyBag* 去得到想要得到的特性

## 


## CoCreateInstance
Input: 想要建立的特定類型的 ID
Input/Output: 指向類型物件的 pointer (ICreateDevEnum*)


## CreateClassEnumerator
Object: ICreateDevEnum* 指向的物件
Input/Output: 指向一個指向IEnumMoniker的指標 (IEnumMoniker**)


## 
