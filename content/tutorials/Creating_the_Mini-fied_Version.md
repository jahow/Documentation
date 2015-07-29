---
ID_PAGE: 22641
PG_TITLE: Creating the Mini-fied Version
---
To create the minified version of Babylon.js you just have to 
use [gulp](https://github.com/BabylonJS/Babylon.js/tree/master/Tools/Gulp)

But you may want to work with all basic files. In this case, please download the code and use the following includes (be aware to have the babylon folder at the root of your site. If you want to use your own shaders in this case, you just have to reference them with a "./" at beginning):

```
    <script src="Babylon/Math/babylon.math.js"></script>
    <script src="Babylon/Tools/babylon.database.js"></script>
    <script src="Babylon/Tools/babylon.tools.tga.js"></script>
    <script src="Babylon/Tools/babylon.tools.dds.js"></script>
    <script src="Babylon/Tools/babylon.smartCollection.js"></script>
    <script src="Babylon/Tools/babylon.smartArray.js"></script>
    <script src="Babylon/Tools/babylon.tools.js"></script>
    <script src="Babylon/babylon.engine.js"></script>
    <script src="Babylon/babylon.node.js"></script>
    <script src="Babylon/Tools/babylon.filesInput.js"></script>
    <script src="Babylon/Collisions/babylon.pickingInfo.js"></script>
    <script src="Babylon/Culling/babylon.boundingSphere.js"></script>
    <script src="Babylon/Culling/babylon.boundingBox.js"></script>
    <script src="Babylon/Culling/babylon.boundingInfo.js"></script>
    <script src="Babylon/Mesh/babylon.abstractMesh.js"></script>
    <script src="Babylon/Lights/babylon.light.js"></script>
    <script src="Babylon/Lights/babylon.pointLight.js"></script>
    <script src="Babylon/Lights/babylon.spotLight.js"></script>
    <script src="Babylon/Lights/babylon.hemisphericLight.js"></script>
    <script src="Babylon/Lights/babylon.directionalLight.js"></script>
    <script src="Babylon/Lights/Shadows/babylon.shadowGenerator.js"></script>
    <script src="Babylon/Collisions/babylon.collider.js"></script>
    <script src="Babylon/Collisions/babylon.collisionCoordinator.js"></script>
    <script src="Babylon/Collisions/babylon.collisionWorker.js"></script>
    <script src="Babylon/Cameras/babylon.camera.js"></script>
    <script src="Babylon/Cameras/babylon.targetCamera.js"></script>
    <script src="Babylon/Cameras/babylon.followCamera.js"></script>
    <script src="Babylon/Cameras/babylon.freeCamera.js"></script>
    <script src="Babylon/Cameras/babylon.touchCamera.js"></script>
    <script src="Babylon/Cameras/babylon.arcRotateCamera.js"></script>
    <script src="Babylon/Cameras/babylon.deviceOrientationCamera.js"></script>
    <script src="Babylon/Tools/babylon.gamepads.js"></script> 
    <script src="Babylon/Cameras/babylon.gamepadCamera.js"></script>
    <script src="Babylon/Rendering/babylon.renderingManager.js"></script>
    <script src="Babylon/Rendering/babylon.renderingGroup.js"></script>
    <script src="Babylon/babylon.scene.js"></script>
    <script src="Babylon/Mesh/babylon.vertexBuffer.js"></script>
    <script src="Babylon/Mesh/babylon.instancedMesh.js"></script>
    <script src="Babylon/Mesh/babylon.mesh.js"></script>
    <script src="Babylon/Mesh/babylon.groundMesh.js"></script>
    <script src="Babylon/Mesh/babylon.subMesh.js"></script>
    <script src="Babylon/Materials/textures/babylon.baseTexture.js"></script>
    <script src="Babylon/Materials/textures/babylon.texture.js"></script>
    <script src="Babylon/Materials/textures/babylon.cubeTexture.js"></script>
    <script src="Babylon/Materials/textures/babylon.renderTargetTexture.js"></script>
    <script src="Babylon/Materials/textures/procedurals/babylon.proceduralTexture.js"></script>
    <script src="Babylon/Materials/textures/procedurals/babylon.standardProceduralTexture.js"></script>
    <script src="Babylon/Materials/textures/procedurals/babylon.customProceduralTexture.js"></script>
    <script src="Babylon/Materials/textures/babylon.mirrorTexture.js"></script>
    <script src="Babylon/Materials/textures/babylon.dynamicTexture.js"></script>
    <script src="Babylon/Materials/textures/babylon.videoTexture.js"></script>
    <script src="Babylon/Materials/babylon.effect.js"></script>
    <script src="Babylon/Materials/babylon.material.js"></script>
    <script src="Babylon/Materials/babylon.standardMaterial.js"></script>
    <script src="Babylon/Materials/babylon.multiMaterial.js"></script>
    <script src="Babylon/Loading/babylon.sceneLoader.js"></script>
    <script src="Babylon/Loading/Plugins/babylon.babylonFileLoader.js"></script>
    <script src="Babylon/Sprites/babylon.spriteManager.js"></script>
    <script src="Babylon/Sprites/babylon.sprite.js"></script>
    <script src="Babylon/Layer/babylon.layer.js"></script>
    <script src="Babylon/Particles/babylon.particle.js"></script>
    <script src="Babylon/Particles/babylon.particleSystem.js"></script>
    <script src="Babylon/Animations/babylon.animation.js"></script>
    <script src="Babylon/Animations/babylon.animatable.js"></script>
    <script src="Babylon/Animations/babylon.easing.js"></script>
    <script src="Babylon/Culling/Octrees/babylon.octree.js"></script>
    <script src="Babylon/Culling/Octrees/babylon.octreeBlock.js"></script>
    <script src="Babylon/Bones/babylon.bone.js"></script>
    <script src="Babylon/Bones/babylon.skeleton.js"></script>
    <script src="Babylon/PostProcess/babylon.postProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.postProcessManager.js"></script>
    <script src="Babylon/PostProcess/babylon.passPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.blurPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.refractionPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.blackAndWhitePostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.convolutionPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.filterPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.fxaaPostProcess.js"></script>
    <script src="Babylon/LensFlare/babylon.lensFlare.js"></script>
    <script src="Babylon/LensFlare/babylon.lensFlareSystem.js"></script>
    <script src="Babylon/Physics/Plugins/babylon.cannonJSPlugin.js"></script>
    <script src="Babylon/Physics/Plugins/babylon.oimoJSPlugin.js"></script>
    <script src="Babylon/Physics/babylon.physicsEngine.js"></script>
    <script src="Babylon/Tools/babylon.sceneSerializer.js"></script>
    <script src="Babylon/Mesh/babylon.csg.js"></script>
    <script src="Babylon/PostProcess/babylon.vrDistortionCorrectionPostProcess.js"></script>
    <script src="Babylon/Tools/babylon.virtualJoystick.js"></script>
    <script src="Babylon/Cameras/babylon.virtualJoysticksCamera.js"></script>
    <script src="Babylon/Materials/babylon.shaderMaterial.js"></script>
    <script src="Babylon/Mesh/babylon.mesh.vertexData.js"></script>
    <script src="Babylon/PostProcess/babylon.anaglyphPostProcess.js"></script>
    <script src="Babylon/Tools/babylon.tags.js"></script>
    <script src="Babylon/Tools/babylon.andOrNotEvaluator.js"></script>
    <script src="Babylon/PostProcess/RenderPipeline/babylon.postProcessRenderPass.js"></script>
    <script src="Babylon/PostProcess/RenderPipeline/babylon.postProcessRenderEffect.js"></script>
    <script src="Babylon/PostProcess/RenderPipeline/babylon.postProcessRenderPipeline.js"></script>
    <script src="Babylon/PostProcess/RenderPipeline/babylon.postProcessRenderPipelineManager.js"></script>
    <script src="Babylon/PostProcess/babylon.displayPassPostProcess.js"></script>
    <script src="Babylon/Rendering/babylon.boundingBoxRenderer.js"></script>
    <script src="Babylon/Actions/babylon.condition.js"></script>
    <script src="Babylon/Actions/babylon.action.js"></script>
    <script src="Babylon/Actions/babylon.actionManager.js"></script>
    <script src="Babylon/Actions/babylon.interpolateValueAction.js"></script>
    <script src="Babylon/Actions/babylon.directActions.js"></script>
    <script src="Babylon/Mesh/babylon.geometry.js"></script>
    <script src="Babylon/Mesh/babylon.linesMesh.js"></script>
    <script src="Babylon/Rendering/babylon.outlineRenderer.js"></script>
    <script src="Babylon/Tools/babylon.assetsManager.js"></script>
    <script src="Babylon/Cameras/VR/babylon.vrDeviceOrientationCamera.js"></script>
    <script src="Babylon/Cameras/VR/babylon.webVRCamera.js"></script>
    <script src="Babylon/Tools/babylon.sceneOptimizer.js"></script>
    <script src="Babylon/Mesh/babylon.meshLODLevel.js"></script>
    <script src="Babylon/Audio/babylon.audioEngine.js"></script>
    <script src="Babylon/Audio/babylon.sound.js"></script>
    <script src="Babylon/Audio/babylon.soundtrack.js"></script>
    <script src="Babylon/Debug/babylon.debugLayer.js"></script>
    <script src="Babylon/Materials/Textures/babylon.rawTexture.js"></script>
    <script src="Babylon/Mesh/babylon.polygonMesh.js"></script>
    <script src="Babylon/Mesh/babylon.meshSimplification.js"></script>
    <script src="Babylon/Audio/babylon.analyser.js"></script>
    <script src="Babylon/Rendering/babylon.depthRenderer.js"></script>
    <script src="Babylon/PostProcess/babylon.ssaoRenderingPipeline.js"></script> 
    <script src="Babylon/PostProcess/babylon.volumetricLightScatteringPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.lensRenderingPipeline.js"></script>
    <script src="Babylon/PostProcess/babylon.colorCorrectionPostProcess.js"></script>
    <script src="Babylon/PostProcess/babylon.stereoscopicInterlacePostProcess.js"></script>
    <script src="Babylon/Cameras/babylon.stereoscopicCameras.js"></script>
    <script src="Babylon/PostProcess/babylon.hdrRenderingPipeline.js"></script>
```

When working with all files, you can provide the following information to the engine:

* BABYLON.Engine.CodeRepository: By default, this value points to "/BABYLON/"
* BABYLON.Engine.ShadersRepository: By default, this value points to "/BABYLON/Shaders/"