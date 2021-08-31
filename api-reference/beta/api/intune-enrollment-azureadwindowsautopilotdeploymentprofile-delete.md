---
title: Удаление azureADWindowsAutopilotDeploymentProfile
description: Удаляет azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0eb50b3e66f90b88089786e6fc44deb95c58ece4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58765213"
---
# <a name="delete-azureadwindowsautopilotdeploymentprofile"></a>Удаление azureADWindowsAutopilotDeploymentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Удаляет [azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```



