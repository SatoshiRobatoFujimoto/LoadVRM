# 1 VRMSpringBoneをDynamicBoneに置換する方法
大まかな設定反映になります。細かい設定はDynamicBoneの各パラメータをいじってください。<br>

## 1.1 VRMSpringBoneの設定を出力する
1.HierarchyにVRMSpringBone、Colliderの設定を出力したいモデルを配置します<br>
例）VRoidStudioで作成し、Blenderで編集前のVRMファイル<br>
注意）モデルはシーン上に1体だけおいてください。<br>
2.メニューにて、UniVRM-(バージョン名)→VRMSpringBone→ExportSettingを選択します<br>
3.exportボタンを押します<br>
4.Colliderフォルダ、SpringBoneフォルダに設定値が出力された.assetファイルが作成されていればOKです。<br>

## 1.2 DyanamicBoneにVRMSpringBoneの設定を反映、置換する
1.Colliderフォルダ、SpringBoneフォルダにVRMSpringBone、Colliderの設定ファイルがあることを確認します。<br>
2.HierarchyにVRMSpringBone、Colliderの設定を反映したいモデルを配置します<br>
注意1）fbxファイルは一度、UniVRM-(バージョン名)→ExportHumanoidを実行してVRMファイル化してください<br>
注意2）モデルはシーン上に1体だけおいてください。<br>

3.メニューにて、UniVRM-(バージョン名)→ReplaceBone→SpringBoneToDynamicBoneを選択します<br>
4.Applyボタンを押します<br>
5.モデル上のsecondaryにDynamicBone、各ボーンにDynamicBoneColliderが反映されていればOKです。<br>

# 2 DynamicBoneをVRMSpringBoneに置換する方法
大まかな設定反映になります。細かい設定はVRMSpringBoneの各パラメータをいじってください。<br>

## 2.1 DynamicBoneの設定を出力する
1.HierarchyにDynamicBone、Colliderの設定を出力したいモデルを配置します<br>
注意1）DynamicBoneスクリプトはsecondaryオブジェクト以外からは読み出されません。<br>
注意2）モデルはシーン上に1体だけおいてください。<br>
2.メニューにて、UniVRM-(バージョン名)→DynamicBone→ExportSettingを選択します<br>
3.exportボタンを押します<br>
4.Colliderフォルダ、DynamicBoneフォルダに設定値が出力された.assetファイルが作成されていればOKです。<br>

## 2.1 VRMSpringBoneにDyanamicBoneの設定を反映、置換する
1.Colliderフォルダ、DynamicBoneフォルダにDynamicBone、Colliderの設定ファイルがあることを確認します。<br>
2.HierarchyにDynamicBone、Colliderの設定を反映したいモデルを配置します<br>
注意1）fbxファイルは一度、UniVRM-(バージョン名)→ExportHumanoidを実行してVRMファイル化してください<br>
注意2）モデルはシーン上に1体だけおいてください。<br>

3.メニューにて、UniVRM-(バージョン名)→ReplaceBone→DynamicBoneToSpringBoneを選択します<br>
4.Applyボタンを押します<br>
5.モデル上のsecondaryにVRMSpringBone、各ボーンにVRMSpringBoneColliderが反映されていればOKです。<br>
