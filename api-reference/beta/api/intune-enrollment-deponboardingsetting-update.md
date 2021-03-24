---
title: Обновление depOnboardingSetting
description: Обновление свойств объекта depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36e173595f1199000f912c3ba4ff8a96e99df8b9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135672"
---
# <a name="update-deponboardingsetting"></a>Обновление depOnboardingSetting

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)

В следующей таблице показаны свойства, необходимые при создании [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID объекта.|
|appleIdentifier|String|ID Apple, используемый для получения текущего маркера.|
|tokenExpirationDateTime|DateTimeOffset|По истечении срока действия маркера.|
|lastModifiedDateTime|DateTimeOffset|Когда служба была на борту.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Когда служба последний раз синхронизирована с Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Когда Intune в последний раз запрашивала синхронизацию.|
|shareTokenWithSchoolDataSyncService|Boolean|Включено ли совместное использование маркеров Dep с помощью службы синхронизации данных школы.|
|lastSyncErrorCode|Int32|Код ошибки, сообщаемой Apple во время последней синхронизации dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md);|Получает или задает тип маркера Dep. Возможные значения: `none`, `dep`, `appleSchoolManager`.|
|tokenName|Строка|Friendly Name for Dep Token|
|syncedDeviceCount|Int32|Получает синхронизированное количество устройств|
|dataSharingConsentGranted|Boolean|Согласие, предоставленное для обмена данными с службой Apple Dep|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




