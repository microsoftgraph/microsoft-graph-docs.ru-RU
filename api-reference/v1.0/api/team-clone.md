---
title: Клонирование команды
description: Создание копии команды. Эта операция также создает копию соответствующей группы.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5462a6aec6be8e284a1a4f88f902e0af92b5f8e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978533"
---
# <a name="clone-a-team"></a>Клонирование команды

Пространство имен: microsoft.graph



Создание копии [команды](../resources/team.md). Эта операция также создает копию соответствующей [группы](../resources/group.md).
Вы можете указать, какие части команды необходимо клонировать:

- **Apps** — копирует приложения Microsoft Teams, которые установлены в команде. 
- **channels** — копирует структуру канала (но не сообщения в канале).
- **Members (участники** ) — копирует участников и владельцев группы.
- **Settings** — копирует все параметры в группе, а также параметры группы ключей.
- **вкладки** — копирует вкладки в каналах.

Когда вкладки клонированы, они помещаются в ненастроенное состояние, которые отображаются на панели вкладок в Microsoft Teams, и при первом их открытии вы увидите экран Конфигурация. (Если пользователь, открывающий вкладку, не имеет разрешения на настройку приложений, они увидят сообщение о том, что вкладка еще не настроена.)

Клонирование является длительной операцией.
После возврата клона POST необходимо получить [операцию](../resources/teamsasyncoperation.md) , чтобы убедиться, что он "работает" или "выполнено" или "Failed". Вы должны продолжать работу, пока не запустятся состояние "работает". Рекомендуемая задержка между возвратами составляет 5 секунд.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All, Directory.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений                            | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Тело запроса

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|classification|Строка (необязательно)|Описывает классификацию для группы (например, снижение, среднее или высокое влияние на бизнес). Если классификация не указана, то классификация будет скопирована из исходной группы или группы.|
|description|Строка (необязательно)|Необязательное описание для группы. Если это свойство не задано, оно будет оставлено пустым.|
|displayName|String|Отображаемое имя для группы. Это свойство необходимо при создании группы. Оно не может быть удалено во время обновления. Поддерживает параметры $filter и $orderby.|
|mailNickname|String|Почтовый псевдоним для группы (уникальный в организации). Это свойство должно быть указано при создании группы. Поддерживает параметр $filter. Если это свойство не задано, оно будет вычислено в displayName. Известная проблема: данное свойство в настоящее время игнорируется.|
|партстоклоне| [клонаблетеампартс](../resources/clonableteamparts.md) |Разделенный запятыми список частей, которые необходимо клонировать. Юридическими частями являются "приложения, вкладки, параметры, каналы, элементы".|
|visibility|[объекта teamvisibilitytype](../resources/teamvisibilitytype.md) (необязательно)| Задает видимость группы. Возможные значения: **Private**, **Public**. Если параметр Visibility не указан, то видимость будет скопирована из исходной группы или группы. Если **Группа является** клонированной, параметр видимости игнорируется, и для отображения новой группы будет задано значение значение hiddenmembership.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвратит `202 Accepted` код отклика с расположением: Header, указывающий на ресурс [Operation](../resources/teamsasyncoperation.md) .
После завершения операции ресурс Operation сообщит вам идентификатор созданной команды.

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

---


#### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
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

