---
title: Обновление windowsDriverUpdateProfile
description: Обновление свойств объекта WindowsDriverUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 58b4b986183f4ac5247103a8d214e7c488811cc2
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629493"
---
# <a name="update-windowsdriverupdateprofile"></a>Обновление windowsDriverUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для [объекта WindowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) .

В следующей таблице показаны свойства, необходимые при создании [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID Intune политики.|
|displayName|Строка|Имя отображения для профиля.|
|description|Строка|Описание профиля, указанного пользователем.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Тип утверждения профиля обновления драйвера. Например, ручное или автоматическое утверждение. Возможные значения: `manual`, `automatic`.|
|deviceReporting|Int32|Количество устройств, сообщив об этом профиле|
|newUpdates|Int32|Количество новых обновлений драйвера, доступных для этого профиля.|
|deploymentDeferralInDays|Int32|Параметры отсрочки развертывания в днях, применимые только при автоматическом утверждении ApprovalType.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого объекта обновления драйвера.|
|inventorySyncStatus|[windowsDriverUpdateProfileInventorySyncStatus](../resources/intune-softwareupdate-windowsdriverupdateprofileinventorysyncstatus.md)|Состояние синхронизации инвентаризации драйверов для этого профиля.|



## <a name="response"></a>Отклик
В случае успешной `200 OK` работы этот метод возвращает код отклика и обновленный [объект WindowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "approvalType": "automatic",
  "deviceReporting": 15,
  "newUpdates": 10,
  "deploymentDeferralInDays": 8,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "inventorySyncStatus": {
    "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "driverInventorySyncState": "success"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 727

{
  "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
  "id": "55bcc52a-c52a-55bc-2ac5-bc552ac5bc55",
  "displayName": "Display Name value",
  "description": "Description value",
  "approvalType": "automatic",
  "deviceReporting": 15,
  "newUpdates": 10,
  "deploymentDeferralInDays": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "inventorySyncStatus": {
    "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
    "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
    "driverInventorySyncState": "success"
  }
}
```




