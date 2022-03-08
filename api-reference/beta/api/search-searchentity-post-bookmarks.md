---
title: Создание закладки
description: Создайте новый объект закладки.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f935c97a966755a3cdb519cf5d6e1ff6bf76dd96
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339119"
---
# <a name="create-bookmark"></a>Создание закладки
Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект закладки](../resources/search-bookmark.md) .

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
}-->
```http
POST /search/bookmarks
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса указать JSON-представление объекта [закладки](../resources/search-bookmark.md) .

В следующей таблице показаны свойства, доступные при создании [закладки](../resources/search-bookmark.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя закладки, отображаемая в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|description|String|Описание закладки, показанное на странице результатов поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|ССЫЛКА URL-адреса закладок. Когда пользователи щелкают эту закладки в результатах поиска, они перейдут на этот URL-адрес. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|categories|Коллекция String|Категории, обычно используемые для описания этой закладки. Например, ИТ и HR.|
|availabilityStartDateTime|DateTimeOffset|Время начала появления закладки в результате поиска. Установите, как `null` всегда доступно.|
|availabilityEndDateTime|DateTimeOffset|Время, когда закладки перестанут отображаться в результате поиска. Установите, как `null` всегда доступно.|
|LanguageTags|Коллекция объектов string|Список стран или регионов, которые могут просмотреть эту закладку.|
|платформы|коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, способных просматривать эту закладку. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты закладки для разных стран или устройств. Используйте, когда необходимо показывать пользователям различные контенты на основе их устройства, страны или региона или обоих. Параметры даты и группы будут применяться для всех вариантов.|
|powerAppIds|Коллекция объектов string|Список Power Apps, связанных с этой закладкой. Если пользователи добавляют существующие Power Apps в закладки, они могут выполнять задачи, например вводить время отпуска или сообщать о расходах на странице результатов поиска.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают эту закладку, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние закладки. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать эту закладку.|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `201 Created` ответа с кодом созданной закладки.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": null,
  "availabilityEndDateTime": null,
  "platforms": ["windows"],
  "targetedVariations": [
    {
      "languageTag": "es-ES",
      "displayName": "Sitio de instalación Contoso",
      "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
    }
  ],
  "groupIds": ["groupId"],
  "powerAppIds": ["powerAppId"],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookmark-from-bookmarks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookmark-from-bookmarks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookmark-from-bookmarks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookmark-from-bookmarks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-bookmark-from-bookmarks-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-bookmark-from-bookmarks-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

