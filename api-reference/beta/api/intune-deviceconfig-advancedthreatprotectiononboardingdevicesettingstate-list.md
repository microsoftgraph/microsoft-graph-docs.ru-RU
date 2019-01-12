---
title: Список advancedThreatProtectionOnboardingDeviceSettingStates
description: Свойства списка и связей объектов advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 018ab29513b9a44d4068cc63b67b6432cc03656d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983536"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a>Список advancedThreatProtectionOnboardingDeviceSettingStates

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Свойства списка и связей объектов [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
      "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```





