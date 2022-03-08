---
title: Обновление закладки
description: Обновление свойств объекта закладки.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5eddbf0551e7acddd1af15123c927201b3aba73d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339131"
---
# <a name="update-bookmark"></a>Обновление закладки
Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [закладки](../resources/search-bookmark.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /search/bookmarks/{bookmarksId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса указать JSON-представление объекта [закладки](../resources/search-bookmark.md) . Поставляем значения для соответствующих полей, которые должны быть обновлены. Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений в других значениях свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.
>**Примечание:** Обновления свойств коллекции обновят всю коллекцию. Любые обновления коллекции, например ключевые слова или категории, полностью заменят коллекцию.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя закладки, отображаемая в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|description|String|Описание закладки, показанное на странице результатов поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|ССЫЛКА URL-адреса закладок. Когда пользователи щелкают эту закладки в результатах поиска, они перейдут на этот URL-адрес. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|categories|Коллекция String|Категории, обычно используемые для описания этой закладки. Например, ИТ и HR.|
|availabilityStartDateTime|DateTimeOffset|Время начала появления закладки в результате поиска. Установите, как `null` всегда доступно.|
|availabilityEndDateTime|DateTimeOffset|Время, когда закладки перестанут отображаться в результате поиска. Установите, как `null` всегда доступно.|
|LanguageTags|Коллекция String|Список стран или регионов, которые могут просмотреть эту закладку.|
|платформы|коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, способных просматривать эту закладку. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты закладки для разных стран или устройств. Используйте, когда необходимо показывать пользователям различные контенты на основе их устройства, страны или региона или обоих. Параметры даты и группы будут применяться для всех вариантов.|
|powerAppIds|Коллекция строк|Список Power Apps, связанных с этой закладкой. Если пользователи добавляют существующие Power Apps в закладки, они могут выполнять задачи, например вводить время отпуска или сообщать о расходах на странице результатов поиска.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают эту закладку, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние закладки. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать эту закладку.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookmark"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/search/bookmarks/{bookmarksId}
Content-Type: application/json

{
  "description": "Book a fancy vacation in Tuscany or browse museums in Florence."
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookmark-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookmark-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookmark-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookmark-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookmark-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookmark-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

