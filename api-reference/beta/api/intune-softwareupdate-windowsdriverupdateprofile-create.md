---
title: Создание windowsDriverUpdateProfile
description: Создайте новый объект WindowsDriverUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 456928b16a18ff3bedb4d743bd39e95e07e30c43
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346355"
---
# <a name="create-windowsdriverupdateprofile"></a>Создание windowsDriverUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте [новый объект WindowsDriverUpdateProfile.](../resources/intune-softwareupdate-windowsdriverupdateprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsDriverUpdateProfiles
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для объекта WindowsDriverUpdateProfile.

В следующей таблице показаны свойства, необходимые при создании windowsDriverUpdateProfile.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID политики Intune.|
|displayName|String|Имя отображения для профиля.|
|description|Строка|Описание профиля, указанного пользователем.|
|approvalType|[driverUpdateProfileApprovalType](../resources/intune-softwareupdate-driverupdateprofileapprovaltype.md)|Тип утверждения профиля обновления драйвера. Например, ручное или автоматическое утверждение. Возможные значения: `manual`, `automatic`.|
|deviceReporting|Int32|Количество устройств, сообщив об этом профиле|
|newUpdates|Int32|Количество новых обновлений драйвера, доступных для этого профиля.|
|deploymentDeferralInDays|Int32|Параметры отсрочки развертывания в днях, применимые только при автоматическом утверждении ApprovalType.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого объекта обновления драйвера.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles
Content-type: application/json
Content-length: 322

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
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

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
  ]
}
```




