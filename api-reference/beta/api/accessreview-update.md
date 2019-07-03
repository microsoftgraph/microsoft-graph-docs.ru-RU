---
title: Обновление Акцессревиев
description: В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0072beb769c99e0da63fae0e2fff258b09e986fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439989"
---
# <a name="update-accessreview"></a>Обновление Акцессревиев

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы изменить одно или несколько его свойств.

Этот API не предназначен для изменения рецензентов или решений проверки.  Чтобы изменить проверяющих, используйте API [аддревиевер](accessreview-addreviewer.md) или [ремоверевиевер](accessreview-removereviewer.md) .  Чтобы остановить уже начатую проверку или уже запущенный экземпляр повторяющегося рецензирования, используйте API [Stop](accessreview-stop.md) . Чтобы применить решения к целевой группе или правам доступа приложения, используйте API [Apply](accessreview-apply.md) . 


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление параметров объекта [акцессревиев](../resources/accessreview.md) в формате JSON.

В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Имя проверки доступа.  |
| `startDateTime`           |`DateTimeOffset`                                                | Дата и время, когда выполняется запланированное начало проверки.  Это должна быть Дата в будущем.   |
| `endDateTime`             |`DateTimeOffset`                                                | Дата и время окончания запланированного рассмотрения. Это должен быть по крайней мере один день позже даты начала.   |
| `description`             |`String`                                                        | Описание, которое будет отображаться для рецензентов. |



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `204, Accepted` код отклика и объект [акцессревиев](../resources/accessreview.md) в тексте отклика.

## <a name="example"></a>Пример

Это пример обновления доступа к одноразовой (неповторной) проверке доступа.

##### <a name="request"></a>Запрос
В теле запроса добавьте представление новых свойств объекта [акцессревиев](../resources/accessreview.md) в формате JSON.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
