# Learning Unit (LU)

## Introduction

The Learning Unit is the minimum unit of information in eLIS. For example, let's say you're cooking a chocolate cake. One of the minimum units of information would be the chocolate itself. The Learning Unit of the chocolate, for this use case, could contain information about the type of chocolate, a description and even an image.

We can combine several Learning Units to get something more meaningful: knowledge. If the knowledge we want to have is how to bake the chocolate cake, we would combine the chocolate LU with other possible LUs such as the sugar, or the spoon to measure the sugar.

## Structure

These are the LU fields:

* **id**: The LU identifier. You can choose any format of your choice: for example, it can be a simple number, a hash or an URI. The only limitation is that it must be unique when using along with other LUs.
* **key**: String. The key field also identifies the LU, but it has to be a String.
* **content**:
* **value**:
* **media**:
* **author**:

This would be the equivalent structure in JSON format:

```js
{
  id: '',
  key: '',
  content: '',
  value: '',
  media: [],
  author: [] // optional
}
```

## Combining LUs

The Learning Units can be combined in three different ways. In eLIS, the final result (the knowlege) is created by combining two or more Learning Units. But this combination is limited to three types: **match**, **group** and **build**. These combinations are called "Learning Connections".