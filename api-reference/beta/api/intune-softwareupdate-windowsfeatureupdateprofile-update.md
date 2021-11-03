---
title: Обновление windowsFeatureUpdateProfile
description: Обновление свойств объекта windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83721b5a2bcb64fa03359272279e0c0ea6bbe381
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695435"
---
# <a name="update-windowsfeatureupdateprofile"></a>Обновление windowsFeatureUpdateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)

В следующей таблице показаны свойства, необходимые при создании [windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта.|
|displayName|String|Имя отображения профиля.|
|description|String|Описание профиля, указанного пользователем.|
|featureUpdateVersion|String|Версия обновления функций, которая будет развернута на устройствах, на которые ориентирован этот профиль. Версия может быть любой поддерживаемой версией, например 1709, 1803 или 1809 и так далее.|
|rolloutSettings|[windowsUpdateRolloutSettings](../resources/intune-softwareupdate-windowsupdaterolloutsettings.md)|Параметры обновления windows, включая время начала предложения, время конечной даты предложения и дни между каждым набором предложений.|
|createdDateTime|DateTimeOffset|Время создания профиля.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения профиля.|
|roleScopeTagIds|Коллекция строк|Список тегов области для этого объекта обновления функций.|
|deployableContentDisplayName|String|Удобное отображаемое имя развернутого контента профиля обновления качества|
|endOfSupportDate|DateTimeOffset|Последняя поддерживаемая дата обновления функций|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "rolloutSettings": {
    "@odata.type": "microsoft.graph.windowsUpdateRolloutSettings",
    "offerStartDateTimeInUTC": "2017-01-01T00:01:16.3697768-08:00",
    "offerEndDateTimeInUTC": "2016-12-31T23:58:15.1925199-08:00",
    "offerIntervalInDays": 3
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "rolloutSettings": {
    "@odata.type": "microsoft.graph.windowsUpdateRolloutSettings",
    "offerStartDateTimeInUTC": "2017-01-01T00:01:16.3697768-08:00",
    "offerEndDateTimeInUTC": "2016-12-31T23:58:15.1925199-08:00",
    "offerIntervalInDays": 3
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```



