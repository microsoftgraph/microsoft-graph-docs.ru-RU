---
title: Создание QNA
description: Создайте новый объект qna.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d3b2266238a74b052aba433c75e5b91d08669386
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602723"
---
# <a name="create-qna"></a>Создание QNA
Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект qna](../resources/search-qna.md) .

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
}
-->
``` http
POST /search/qnas
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [Qna](../resources/search-qna.md) в формате JSON.

В следующей таблице показаны свойства, доступные при создании [QNA](../resources/search-qna.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Вопрос, отображаемый в результатах поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|description|Строка|Ответ, отображаемый в результатах поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Ссылка на URL-адрес Qna. Когда пользователи щелкают этот QNA в результатах поиска, они будут переходить по этому URL-адресу. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|availabilityStartDateTime|DateTimeOffset|Метка времени, когда qna начнет отображаться в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|availabilityEndDateTime|DateTimeOffset|Метка времени остановки qna в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|languageTags|Коллекция строк|Список стран или регионов, которые могут просматривать этот qna.|
|Платформ|Коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, которые могут просматривать этот QNA. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[Коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты QNA для разных стран или устройств. Используйте, если необходимо показывать пользователям разные материалы в зависимости от их устройства, страны или региона или и того, и другого. Параметры даты и группы будут применяться ко всем вариантам.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые инициирует отображение этого QNA в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние qna. Возможные значения: `published`, `draft`, или `excluded``unknownFutureValue`.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать этот qna.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` ответа с идентификатором созданного вопроса и ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_qna_from_qnas"
}-->
```http
POST https://graph.microsoft.com/beta/search/qnas
Content-Type: application/json

{
  "displayName": "Global Country Holidays",
  "webUrl": "http://www.contoso.com/",
  "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>",
  "keywords":  {
    "keywords": ["new years day", "martin luther king day", "presidents day", "memorial day", "independence day", "labor day", "thanksgiving", "christmas"],
    "reservedKeywords": ["holidays", "paid days off"],
    "matchSimilarKeywords": true
  },
  "availabilityStartDateTime": "2020-09-21T20:01:37Z",
  "availabilityEndDateTime": "2021-12-31T20:01:37Z",
  "languageTags": ["en-us"],
  "platforms": ["ios"],
  "state": "published"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-qna-from-qnas-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-qna-from-qnas-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-qna-from-qnas-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-qna-from-qnas-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-qna-from-qnas-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-qna-from-qnas-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.qna"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

