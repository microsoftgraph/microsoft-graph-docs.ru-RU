---
title: Обновление depOnboardingSetting
description: Обновление свойства объекта depOnboardingSetting.
ms.openlocfilehash: 931df96b837610044a8c9337fa1fbd5de2a3d52d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074876"
---
# <a name="update-deponboardingsetting"></a>Обновление depOnboardingSetting

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойства объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .

В следующей таблице показаны свойства, которые необходимы для создания [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|appleIdentifier|String|Apple идентификатор, используемый для получения текущего маркера.|
|tokenExpirationDateTime|DateTimeOffset|Маркер истечения срока действия.|
|lastModifiedDateTime|DateTimeOffset|Когда служба была onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|При последней syned службы с помощью Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Когда Intune запрашивает последней синхронизации.|
|shareTokenWithSchoolDataSyncService|Логический|Ли Dep маркеров общий доступ к включается со службой синхронизации данных School.|
|lastSyncErrorCode|Int32|Код ошибки Apple во время последней синхронизации dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md);|Получает или задает тип токена Dep. Возможные значения: `none`, `dep`, `appleSchoolManager`.|
|tokenName|String|Понятное имя для маркера Dep|
|syncedDeviceCount|Int32|Получает количество синхронизированных устройства|
|defaultProfileDisplayName|String|Получает количество синхронизированных устройства|
|dataSharingConsentGranted|Логический|Предоставляются разрешения для данных, общий доступ к службе Dep Apple|



## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) объекта в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 589

{
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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





