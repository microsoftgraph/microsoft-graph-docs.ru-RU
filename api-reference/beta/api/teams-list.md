---
title: Список команд
description: Перечисление всех команд в организации
author: akhilkohlimicrosoft
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c4a2d90f3c82c7066fee7c98aebbd3ba011c825
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432746"
---
# <a name="list-teams"></a>Список команд

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Перечисление всех [команд](../resources/team.md) в организации.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /teams
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select`, `$top`, `$skiptoken`, `$count` для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |
| Accept  | application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает `200 OK`код ответа и коллекцию объектов [team](../resources/team.md) в теле ответа.

> [!Note]
> В настоящее время этот вызов API возвращает только свойства **id**, **displayName** и **description** [команды](../resources/team.md). Чтобы получить все свойства, воспользуйтесь операцией [Получение команды](../api/team-get.md). 

## <a name="examples"></a>Примеры

### <a name="example-1-get-a-list-of-teams"></a>Пример 1. Получение списка команд

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams
```
---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "Contoso General Team",
      "description": "This is a general Contoso team"
    },
    ,
    {
      "id": "98678abcce0-e65d-44ce-9a49-9980bj8kl0e",
      "displayName": "Contoso API Team",
      "description": "This is Contoso API team"
    }
  ]
}
```

### <a name="example-2-use-filter-and-top-to-get-two-teams-with-a-display-name-that-starts-with-a"></a>Пример 2. Использование параметров $filter и $top для получения двух команд с отображаемым именем, которое начинается с "А"

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->

```http
GET https://graph.microsoft.com/beta/teams?$filter=startswith(displayName, 'A')&$top=2
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "displayName": "A Contoso Team",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    },
    {
      "id": "890972b0cce-e65d-44ce-9a49-568hhsd7n",
      "displayName": "A Contoso Notification Team",
      "description": "This is a notification Contoso team"
    },
  ]
}
```

### <a name="example-3-use-filter-and-select-to-get-id-and-description-for-team-with-displayname-equals-a-contoso-team"></a>Пример 3. Использование параметров $filter и $select для получения ИД и описания команды с отображаемым именем "A Contoso Team" (Команда Contoso)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_teams"
}-->
```http
GET https://graph.microsoft.com/beta/teams?$filter=displayName eq 'A Contoso Team'&$select=id,description
```
---

#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "172b0cce-e65d-44ce-9a49-91d9f2e8493a",
      "description": "This is a Contoso team, used to showcase the range of properties supported by this API"
    }
  ]
}
```


## <a name="see-also"></a>См. также
- [Получение команды](../api/team-get.md)