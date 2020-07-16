---
title: Получение Рапрофиледатабасинтити
description: Чтение свойств и связей объекта Рапрофиледатабасинтити.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0dbd34afd108a50a5e91aac414cc19ecd86282
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124350"
---
# <a name="get-raprofiledatabaseentity"></a>Получение Рапрофиледатабасинтити

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рапрофиледатабасинтити](../resources/intune-rapolicy-raprofiledatabaseentity.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/resourceAccessProfileEntities/{resourceAccessProfileEntitiesId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 856

{
  "value": {
    "@odata.type": "#microsoft.graph.raProfileDatabaseEntity",
    "version": 7,
    "isDeleted": true,
    "softDeletedTime": "2016-12-31T23:59:22.6041454-08:00",
    "displayName": "Display Name value",
    "linkedProfileIds": [
      "5b59ac1a-ac1a-5b59-1aac-595b1aac595b"
    ],
    "profileTypeName": "Profile Type Name value",
    "profileBody": "Profile Body value",
    "profileBodyHash": "Profile Body Hash value",
    "platformType": 12,
    "transformedProfileBody": "Transformed Profile Body value",
    "transformedProfileBodyHash": "Transformed Profile Body Hash value",
    "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
    "profileId": "6389d896-d896-6389-96d8-896396d88963",
    "eTag": "ETag value",
    "schemaVersion": "betaStart",
    "lastModified": "2017-01-01T00:03:14.6651031-08:00"
  }
}
```



