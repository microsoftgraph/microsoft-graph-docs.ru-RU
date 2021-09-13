---
title: Создать VPP токен
description: Создайте новый объект vppToken.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b166f50b35edaabaed47881846f11a428fca4ab6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026408"
---
# <a name="create-vpptoken"></a>Создать VPP токен

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый объект [vppToken](../resources/intune-onboarding-vpptoken.md).

## <a name="prerequisites"></a>Обязательные требования
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
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта VPP токен в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта VPP токен.

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



## <a name="response"></a>Ответ
В случае успешного выполнения данный метод возвращает`201 Created` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
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
HTTP/1.1 201 Created
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




