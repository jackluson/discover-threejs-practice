
- getWorldPosition

getWorldPosition() is a method in the Three.js library that can be called on a Mesh object to return its world position. The world position of an object is its position in the global coordinate system of the scene, taking into account any transformations that may have been applied to its parent objects.


Here's an example of how to use getWorldPosition():


```js
// Assuming you have a Mesh object called "mesh"
const worldPosition = new THREE.Vector3();
mesh.getWorldPosition(worldPosition);
console.log(worldPosition);
```

In this example, we first create a new Vector3 object to store the world position of the mesh. We then call getWorldPosition() on the mesh object, passing in the Vector3 object as an argument. The method updates the Vector3 object with the world position of the mesh. Finally, we log the world position to the console.


Note that if the mesh has a parent object that has been transformed, the world position returned by getWorldPosition() will reflect those transformations. If you need the position relative to the parent object, you can use the position property of the mesh instead.



> https://threejs.org/docs/#api/en/core/Object3D.getWorldPosition
