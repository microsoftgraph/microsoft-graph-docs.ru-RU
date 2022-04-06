---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c22872836de65c59c2714fbdbe53a6885e61c17e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcUserSetting()
displayName := "Example"
requestBody.SetDisplayName(&displayName)
selfServiceEnabled := true
requestBody.SetSelfServiceEnabled(&selfServiceEnabled)
restorePointSetting := msgraphsdk.NewCloudPcRestorePointSetting()
requestBody.SetRestorePointSetting(restorePointSetting)
frequencyInHours := int32(16)
restorePointSetting.SetFrequencyInHours(&frequencyInHours)
userRestoreEnabled := true
restorePointSetting.SetUserRestoreEnabled(&userRestoreEnabled)
localAdminEnabled := false
requestBody.SetLocalAdminEnabled(&localAdminEnabled)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
}
options := &msgraphsdk.CloudPcUserSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
cloudPcUserSettingId := "cloudPcUserSetting-id"
graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById(&cloudPcUserSettingId).Patch(options)


```