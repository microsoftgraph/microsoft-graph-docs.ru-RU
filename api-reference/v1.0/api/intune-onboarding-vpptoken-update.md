---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f57923cee1a6dd261a45d1c31bc3d4ec58e4c59
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026359"
---
# <a name="update-vpptoken"></a>Обновить VPP токен

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).

## <a name="prerequisites"></a>Предварительные требования
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Создается автоматически при создании appleVolumePurchaseProgramToken. Это ключ объекта.|
|organizationName|Строка|Организация, связанная с токеном Apple Volume Purchase Program.|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.|
|appleId|Строка|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|Дата и время завершения срока действия токена Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.|
|токен|Строка|Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.|
|состояние|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Текущее состояние токена Apple Volume Purchase Program. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program. Возможные значения: `none`, `inProgress`, `completed`, `failed`. Возможные значения: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Логическое|Автоматически обновятся все приложения, не только для токена VPP.|
|countryOrRegion|Строка|Автоматически обновятся все приложения, не только для токена VPP.|



## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```




