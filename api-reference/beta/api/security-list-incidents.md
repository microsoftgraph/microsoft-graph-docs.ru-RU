---
title: Получение списка инцидентов
description: Получите список объектов инцидента и их свойств.
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1e0dd929000299770d3e5240905e17890ba2ae7e
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220853"
---
# <a name="list-incidents"></a>Получение списка инцидентов
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [инцидента](../resources/incident.md) и их свойств.

Операция инцидентов списка позволяет сортировать инциденты, чтобы создать информированный ответ на кибербезопасность. Он предоставляет коллекцию инцидентов, которые были помечены в сети, в диапазоне времени, указанном в политике хранения среды. Последние инциденты отображаются в верхней части списка.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Incidents.Read.All, Incidents.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Incidents.Read.All, Incidents.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ: `$count` `$filter` , , , `$skip` `$top` .

Поддержка следующих `$filter` свойств: **assignedTo**, **классификация**, **createdDateTime**, **определение,** **lastUpdateDateTime**, **серьезность** и **состояние**.

Используйте `@odata.nextLink` для pagination.

Ниже приводится пример их использования:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/incidents?$count=true
GET /security/incidents?$filter={property}+eq+'{property-value}'
GET /security/incidents?$top=10
```

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).


## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` инцидентов в тексте [](../resources/incident.md) отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_incident"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/incidents
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.incident",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
        "@odata.type": "#microsoft.graph.incident",
        "id": "2972395",
        "incidentWebUrl": "https://security.microsoft.com/incidents/2972395?tid=12f988bf-16f1-11af-11ab-1d7cd011db47",
        "redirectIncidentId": null,
        "displayName": "Multi-stage incident involving Initial access & Command and control on multiple endpoints reported by multiple sources",
        "createdDateTime": "2021-08-13T08:43:35.5533333Z",
        "lastUpdateDateTime": "2021-09-30T09:35:45.1133333Z",
        "assignedTo": "KaiC@contoso.onmicrosoft.com",
        "classification": "TruePositive",
        "determination": "MultiStagedAttack",
        "status": "Active",
        "severity": "Medium",
        "tags": [
          "Demo"
        ],
        "comments": [
          {
                "comment": "Demo incident",
                "createdBy": "DavidS@contoso.onmicrosoft.com",
                "createdTime": "2021-09-30T12:07:37.2756993Z"
          }
        ]
    }
  ]
}
```

