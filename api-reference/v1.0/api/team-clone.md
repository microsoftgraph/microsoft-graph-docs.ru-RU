---
title: Клонировать команду
description: Создайте копию команды. Эта операция также создает копию соответствующей группы.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5da091152a259a2987b2d99a9082a9f6795a60aa
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973690"
---
# <a name="clone-a-team"></a>Клонировать команду

Пространство имен: microsoft.graph



Создайте копию [команды.](../resources/team.md) Эта операция также создает копию соответствующей [группы.](../resources/group.md)
Можно указать, какие части группы клонировать:

- **приложения** — Microsoft Teams приложения, установленные в команде. 
- **каналы** — копирует структуру канала (но не сообщения в канале).
- **члены** — копирует членов и владельцев группы.
- **параметры** — копирует все параметры в команде, а также ключевые параметры группы.
- **вкладки** — копирует вкладки в каналах.

Когда вкладки клонируют, они помещаются в неконфигурированное состояние — они отображаются на панели вкладок в Microsoft Teams, и при первом их открытие вы будете проходить через экран конфигурации. (Если открывающий вкладку человек не имеет разрешения на настройку приложений, он увидит сообщение, объясняя, что вкладка не настроена.)

Клонирование является длительной операцией.
После возвращения клона POST необходимо получить [](../resources/teamsasyncoperation.md) операцию, чтобы узнать, "запущена" или "успешно" или "не удалось". Вы должны продолжать получать, пока состояние не будет "запущено". Рекомендуемая задержка между GETs — 5 секунд.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Team.Create, Group.ReadWrite.All **, Directory.ReadWrite.All** |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений                            | Team.Create, Group.ReadWrite.All **, Directory.ReadWrite.All** |

> **Примечание**. Разрешения, помеченные **, не поддерживаются и не должны использоваться.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classification|String (необязательный)|Описывает классификацию для группы (например, низкое, среднее или высокое влияние бизнеса). Если классификация не указана, классификация будет скопирована из исходной группы или группы.|
|description|String (необязательный)|Необязательное описание для группы. Если это свойство не указано, оно останется пустым.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|mailNickname|String|Почтовый псевдоним для группы (уникальный в организации). Это свойство должно быть указано при создании группы. Поддерживает параметр $filter. Если это свойство не указано, оно будет вычисляться из displayName. Известная проблема: это свойство в настоящее время игнорируется.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Разделенный запятой список частей для клонирования. Юридическими частями являются "приложения, вкладки, параметры, каналы, члены".|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (необязательный)| Указывает видимость группы. Возможные значения: **Private**, **Public**. Если видимость не указана, видимость будет скопирована из исходной группы или группы. Если клонированная группа является командой **educationClass,** параметр видимости игнорируется, а видимость новой группы будет задана в hiddenMembership.|

## <a name="response"></a>Отклик

В случае успешного использования этот метод возвращает код ответа с заготвом `202 Accepted` Location: header, указывав на [ресурс](../resources/teamsasyncoperation.md) операции.
По завершению операции ресурс операции покажет вам id созданной команды.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clone-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
Ниже представлен пример ответа. Примечание: показанный здесь объект ответа может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

