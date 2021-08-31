---
title: reportRemoteAssistance action
description: Почтовый вызов для отправки полезной нагрузки отчетов
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d00265f73751ac29028aea0ecf9b9d58f721259d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797174"
---
# <a name="reportremoteassistance-action"></a>reportRemoteAssistance action

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Почтовый вызов для отправки полезной нагрузки отчетов

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reportRemoteAssistance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|reportingPayload|[remoteAssistanceReporting](../resources/intune-remoteassistance-remoteassistancereporting.md)|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reportRemoteAssistance

Content-type: application/json
Content-length: 972

{
  "reportingPayload": {
    "@odata.type": "microsoft.graph.remoteAssistanceReporting",
    "id": "Id value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
    "remoteAssistanceSessionType": "fullControl",
    "helperEmail": "Helper Email value",
    "helperTenantId": "Helper Tenant Id value",
    "helperFirstName": "Helper First Name value",
    "helperLastName": "Helper Last Name value",
    "helperDeviceAadId": "Helper Device Aad Id value",
    "helperDeviceName": "Helper Device Name value",
    "helperEnrollmentState": "enrolled",
    "sharerEmail": "Sharer Email value",
    "sharerTenantId": "Sharer Tenant Id value",
    "sharerFirstName": "Sharer First Name value",
    "sharerLastName": "Sharer Last Name value",
    "sharerDeviceAadId": "Sharer Device Aad Id value",
    "sharerDeviceName": "Sharer Device Name value",
    "sharerEnrollmentState": "enrolled"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```



