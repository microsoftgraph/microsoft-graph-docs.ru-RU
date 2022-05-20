---
title: Создание закладки
description: Создайте объект закладки.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 84283c08a8e80427ff34a310cbcae799bd26ecef
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602751"
---
# <a name="create-bookmark"></a>Создание закладки
Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [закладки](../resources/search-bookmark.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Приложение| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |

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
В тексте запроса добавьте представление объекта закладки в формате [JSON.](../resources/search-bookmark.md)

В следующей таблице показаны свойства, доступные при создании [закладки](../resources/search-bookmark.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя закладки, отображаемое в результатах поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|description|Строка|Описание закладки, отображаемое на странице результатов поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Ссылка на URL-адрес закладки. Когда пользователи щелкают эту закладку в результатах поиска, они будут переходить по этому URL-адресу. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|categories|Коллекция String|Категории, часто используемые для описания этой закладки. Например, ИТ-отдел и отдел кадров.|
|availabilityStartDateTime|DateTimeOffset|Метка времени начала отображения закладки в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|availabilityEndDateTime|DateTimeOffset|Метка времени остановки отображения закладки в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|languageTags|Коллекция строк|Список стран или регионов, в которые можно просмотреть эту закладку.|
|Платформ|Коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, которые могут просматривать эту закладку. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[Коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты закладок для разных стран или устройств. Используйте, если необходимо показывать пользователям разные материалы в зависимости от их устройства, страны или региона или и того, и другого. Параметры даты и группы будут применяться ко всем вариантам.|
|powerAppIds|Коллекция String|Список Power Apps, связанных с этой закладкой. Если пользователи добавляют существующие Power Apps в закладку, они могут выполнять такие задачи, как ввод отпуска или отчет о расходах на странице результатов поиска.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают эту закладку, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние закладки. Возможные значения: `published`, `draft`, или `excluded``unknownFutureValue`.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать эту закладку.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика с идентификатором созданной закладки.

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
      "languageTag": "es-es",
      "displayName": "Sitio de instalación Contoso",
      "description": "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
    }
  ],
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

