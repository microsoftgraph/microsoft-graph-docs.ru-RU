---
title: Список teamworkDevices
description: Получите список всех устройств с Microsoft Teams, которые были предусмотрены для клиента.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 91065f7a253e2cd3159cf42d53423c0c381f8a7f
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262699"
---
# <a name="list-teamworkdevices"></a>Список teamworkDevices
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список всех устройств с Microsoft Teams, [которые были](../resources/teamworkdevice.md) предусмотрены для клиента.

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|TeamworkDevice.Read.All, TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/devices
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод `$filter` поддерживает параметры запросов **deviceType**, **hardwareDetail/uniqueId** и **currentUser/id**), `$top``$select``$skipToken` а также параметры запроса [OData](/graph/query-parameters) для настройки ответа.

### <a name="supported-query-patterns"></a>Поддерживаемые шаблоны запросов

| Шаблон                | Синтаксис                                 | Примечания |
| ---------------------- | -------------------------------------- | ----- |
| Pagination на стороне сервера | `@odata.nextLink`                      | В ответе вы получите маркер продолжения, если набор результатов охватывает несколько страниц. |
| Filter                 | `/devices?$filter=deviceType eq 'TeamsRoom'` | Фильтрация устройств в зависимости от категории устройства. |
| Filter                 | `/devices?$filter=hardwareDetail/uniqueId eq 'value'` | Фильтруются устройства на основе **уникальногоid** , назначенного устройству. |
| Filter                 | `/devices?$filter=currentUser/id eq 'value'` |  Фильтруются устройства на основе пользователя, заявляемого на устройстве.|
| Ограничение страницы             | `/devices?$top=10` | Получите устройства с размером страницы 10. Ограничение страницы по умолчанию — 20. Максимальное ограничение страницы — 50. |

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` отклика и коллекцию объектов [teamworkDevice](../resources/teamworkdevice.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_teamworkdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDevice",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teamwork/devices",
  "@odata.count": 2,
  "@odata.nextLink": "/teamwork/devices?$filter=deviceType+eq+Microsoft.Teams.GraphSvc.teamworkDeviceType%collaborationBar%27&$top=2&$skiptoken=%2bRID%3a~z9snAP1BE88Zlz0AAAAADg%3d%3d%23RT%3a1%23TRC%3a3%23RTD%3auCNd2ZP%2fZ5zLgoPeFGRGBTMxMzIuMTcuMzJVMTY7NTc7MjEvNTozNjEyM1sA%23ISV%3a2%23IEO%3a65551%23QCF%3a4%23FPC%3aAggBAAAAADgAAPcAAAAAOAAAAQAAAAA4AAACADiI9AAAAAA4AAACABCP9QAAAAA4AAAEAFEu4AD2AAAAADgAAAQANoXZkfcAAAAAOAAABAAlgIiK",
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamworkDevice",
      "id": "0f3ce432-e432-0f3c-32e4-3c0f32e43c0f",
      "deviceType": "CollaborationBar",
      "hardwareDetail": {
        "serialNumber": "0189",
        "uniqueId": "5abcdefgh",
        "macAddresses": [],
        "manufacturer": "yealink",
        "model": "vc210"
      },
      "notes": "CollaborationBar device.",
      "companyAssetTag": "Tag1",
      "healthStatus": "Healthy",
      "activityState": "Idle",
      "createdDateTime": "2021-06-19T19:01:04.185Z",
      "createdBy": null,
      "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
      "lastModifiedBy": null,
      "currentUser": {
        "id": "2a610f6f-adf6-4205",
        "displayName": "Evan Lewis",
        "userIdentityType": "aadUser"
      }
    },
    {
      "@odata.type": "#microsoft.graph.teamworkDevice",
      "id": "55ab555-e432-0f3c-32e4-3c0f32e43c0f",
      "deviceType": "CollaborationBar",
      "hardwareDetail": {
        "serialNumber": "0189",
        "uniqueId": "5abcdefgh",
        "macAddresses": [],
        "manufacturer": "yealink",
        "model": "vc210"
      },
      "notes": "CollaborationBar device.",
      "companyAssetTag": "Tag2",
      "healthStatus": "Healthy",
      "activityState": "Idle",
      "createdDateTime": "2021-06-10T19:01:04.185Z",
      "createdBy": null,
      "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
      "lastModifiedBy": null,
      "currentUser": {
        "id": "2a610f6f-adf6-4205",
        "displayName": "Evan Lewis",
        "userIdentityType": "aadUser"
      }
    }
  ]
}
```

