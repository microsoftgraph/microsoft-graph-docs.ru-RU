---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: Получение статистики по действиям элемента по интервалу
localization_priority: Normal
ms.openlocfilehash: f9601538d825efe346ab57fdbecd6c74dc9978d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541313"
---
# <a name="get-item-activity-stats-by-interval"></a>Получение статистики по действиям элемента по интервалу

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение [итемактивитистатс][] для действий, выполненных с этим ресурсом в течение указанного интервала времени.

>**Примечание:** Ресурс **итеманалитикс** пока недоступен во всех [национальных развертываниях](/graph/deployments).

Статистические функции аналитики могут быть недоступны для всех типов действий.

[Итемактивитистатс]: ../resources/itemactivitystat.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:--------------------------------------|:-------------------------------------
|Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.
|Для приложений                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-10',interval='day')
GET /sites/{site-id}/getActivitiesByInterval(startDateTime='2016',endDateTime='2017',interval='month')
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-05-01',interval='week')
```

## <a name="function-parameters"></a>Параметры функции

| Параметр      | Тип               | Описание
|:---------------|:-------------------|:---------------------------------------
| startDateTime  | строка (timestamp) | Время начала агрегирования действий.
| endDateTime    | строка (timestamp) | Время окончания агрегирования действий.
| interval       | string             | Интервал объединения.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "get-activities-by-interval" } -->

```http
GET /drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.itemActivityStat)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "startDateTime": "2017-01-01T00:00:00.000Z",
            "endDateTime": "2017-01-02T00:00:00.000Z",
            "delete": {
                "actionCount": 1,
                "actorCount": 1
            },
            "access": {
                "actionCount": 5,
                "actorCount": 3
            }
        },
        {
            "startDateTime": "2017-01-02T00:00:00.000Z",
            "endDateTime": "2017-01-03T00:00:00.000Z",
            "edit": {
                "actionCount": 3,
                "actorCount": 1
            },
            "access": {
                "actionCount": 7,
                "actorCount": 6
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get activities by interval",
  "suppressions": [
    "Error: /api-reference/beta/api/itemactivity-getbyinterval.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
