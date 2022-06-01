---
title: Обновление accessReview (не рекомендуется)
description: В Azure AD проверки доступа обновите существующий объект accessReview, чтобы изменить одно или несколько его свойств.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eb7bc62b0ca05ff985bfb9a06d776d3ed7a2a2eb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819162"
---
# <a name="update-accessreview-deprecated"></a>Обновление accessReview (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки доступа](../resources/accessreviews-root.md) обновите существующий [объект accessReview](../resources/accessreview.md), чтобы изменить одно или несколько его свойств.

Этот API не предназначен для изменения рецензентов или решений проверки.  Чтобы изменить рецензентов, используйте [API addReviewer](accessreview-addreviewer.md) [или removeReviewer](accessreview-removereviewer.md) .  Чтобы остановить уже запущенную разовую проверку или уже запущенный экземпляр повторяющейся проверки, используйте API [остановки](accessreview-stop.md) . Чтобы применить решения к целевой группе или правам доступа к приложению, используйте API [применения](accessreview-apply.md) . 


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров объекта [accessReview в формате](../resources/accessreview.md) JSON.

В следующей таблице показаны свойства, которые можно указать при обновлении accessReview.

| Свойство      | Тип           | Описание                                                                                                |
|:--------------|:---------------|:-----------------------------------------------------------------------------------------------------------|
| displayName   | Строка         | Имя проверки доступа.                                                                                    |
| startDateTime | DateTimeOffset | Дата и время начала проверки.  Это должна быть дата в будущем.                 |
| endDateTime   | DateTimeOffset | Дата и время окончания проверки. Это значение должно быть по крайней мере на один день позже даты начала. |
| description   | Строка         | Описание, отображаемая рецензентам.                                                                 |



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `204 Accepted` отклика и объект [accessReview](../resources/accessreview.md) в тексте отклика.

## <a name="example"></a>Пример

Это пример обновления однофакторной проверки доступа (без повторной проверки).

##### <a name="request"></a>Запрос
В тексте запроса добавьте представление новых свойств объекта [accessReview в формате](../resources/accessreview.md) JSON.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreview-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-accessreview-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


