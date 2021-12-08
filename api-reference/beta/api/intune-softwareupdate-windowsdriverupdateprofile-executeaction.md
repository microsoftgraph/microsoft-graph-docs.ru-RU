---
title: Действие executeAction
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb4a283d2954e0e37828475635727f3fcd6ffe62
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344654"
---
# <a name="executeaction-action"></a>Действие executeAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|[driverApprovalAction](../resources/intune-softwareupdate-driverapprovalaction.md)|Пока не задокументировано.|
|driverIds|Коллекция строк|Н/Д|
|deploymentDate|DateTimeOffset|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успеха это действие возвращает код отклика и `200 OK` [bulkDriverActionResult](../resources/intune-softwareupdate-bulkdriveractionresult.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction

Content-type: application/json
Content-length: 137

{
  "actionName": "decline",
  "driverIds": [
    "Driver Ids value"
  ],
  "deploymentDate": "2016-12-31T23:58:18.3419405-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "microsoft.graph.bulkDriverActionResult",
    "successfulDriverIds": [
      "Successful Driver Ids value"
    ],
    "failedDriverIds": [
      "Failed Driver Ids value"
    ],
    "notFoundDriverIds": [
      "Not Found Driver Ids value"
    ]
  }
}
```




