---
title: Список chromeOSOnboardingSettingses
description: Список свойств и связей объектов chromeOSOnboardingSettings.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11e3fc253e05a570e81cad9e30466f280f18a3d3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117342"
---
# <a name="list-chromeosonboardingsettingses"></a>Список chromeOSOnboardingSettingses

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
      "id": "0344255d-255d-0344-5d25-44035d254403",
      "ownerUserPrincipalName": "Owner User Principal Name value",
      "onboardingStatus": "inprogress",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
    }
  ]
}
```



