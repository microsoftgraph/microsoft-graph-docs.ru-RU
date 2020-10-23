---
title: Список Макоссофтвареупдатекатегорисуммариес
description: Список свойств и связей объектов Макоссофтвареупдатекатегорисуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5059a242979623de599ec5bdf2b1ba4e3c353d4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731808"
---
# <a name="list-macossoftwareupdatecategorysummaries"></a>Список Макоссофтвареупдатекатегорисуммариес

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
      "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
      "displayName": "Display Name value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "updateCategory": "configurationDataFile",
      "successfulUpdateCount": 5,
      "failedUpdateCount": 1,
      "totalUpdateCount": 0,
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





