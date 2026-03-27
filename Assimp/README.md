# Assimp

This project was built with [KalaMake](https://github.com/kalakit/kalamake). Use the `.kmake` and the `zlib` static library with its includes and the kalamake CLI to compile [Assimp](https://github.com/assimp/assimp) from source.

You should also assign these values in your project at runtime
```
//general
scene->mRootNode->SetPropertyFloat(AI_CONFIG_GLOBAL_SCALE_FACTOR_KEY, 1.0f);
scene->mRootNode->SetPropertyFloat(AI_CONFIG_APP_SCALE_KEY, 1.0f);

//fbx
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_READ_ALL_GEOMETRY_LAYERS, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_READ_ALL_MATERIALS, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_READ_MATERIALS, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_READ_TEXTURES, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_OPTIMIZE_EMPTY_ANIMATION_CURVES, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_FBX_CONVERT_TO_M, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_IMPORT_FBX_IGNORE_UP_DIRECTION, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_FBX_USE_SKELETON_BONE_CONTAINER, true);

//post-process
scene->mRootNode->SetPropertyBool(AI_CONFIG_PP_TUV_EVALUATE, true);
scene->mRootNode->SetPropertyInt(AI_CONFIG_PP_LBW_MAX_WEIGHTS, 8);
scene->mRootNode->SetPropertyFloat(AI_CONFIG_PP_FID_ANIM_ACCURACY, 1.0f);
scene->mRootNode->SetPropertyFloat(AI_CONFIG_PP_GSN_MAX_SMOOTHING_ANGLE, 45.0f);
scene->mRootNode->SetPropertyFloat(AI_CONFIG_PP_CT_MAX_SMOOTHING_ANGLE, 45.0f);
scene->mRootNode->SetPropertyInt(AI_CONFIG_PP_SBBC_MAX_BONES, 256);
scene->mRootNode->SetPropertyInt(AI_CONFIG_PP_ICL_PTCACHE_SIZE, 64);

scene->mRootNode->SetPropertyBool(AI_CONFIG_PP_FD_REMOVE, true);
scene->mRootNode->SetPropertyFloat(AI_CONFIG_PP_FD_CHECKAREA, 1e-6f);

scene->mRootNode->SetPropertyBool(AI_CONFIG_PP_PTV_KEEP_HIERARCHY, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_PP_PTV_NORMALIZE, true);
scene->mRootNode->SetPropertyBool(AI_CONFIG_PP_PTV_ADD_ROOT_TRANSFORMATION, true);
```
