---
title: Get mobileAppCategory
description: Чтение свойств и связей объекта mobileAppCategory.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60f9e7597009fbbe86505cd9a7e3790887930787
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450785"
---
# <a name="get-mobileappcategory"></a>Get mobileAppCategory

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 239

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppCategory",
    "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





