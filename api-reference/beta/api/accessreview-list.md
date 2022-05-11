---
title: Перечисление объектов accessReview
description: Получение объектов accessReview для businessFlowTemplate.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8330e5dedcaae077864c556b9def9d09dac2cc8b
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "65314528"
---
# <a name="list-accessreviews"></a>Перечисление объектов accessReview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Получение объектов [accessReview](../resources/accessreview.md) для определенного [объекта businessFlowTemplate](../resources/businessflowtemplate.md). Возвращается список из нуля или более объектов **accessReview** для каждой разной и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-потока.  Обратите внимание, что идентификаторы шаблонов бизнес-потока чувствительны к регистру.

>[!NOTE]
> Если какие-либо проверки доступа, соответствующие фильтру, представляют собой повторяющиеся проверки доступа, будет возвращен один объект **accessReview** , представляющий каждый повторяющийся ряд в целом, в дополнение к любому текущему, прошлому и следующему предстоящему экземпляру. Например, если имеется ежемесячная повторяемая проверка доступа гостевых членов группы A, ежеквартальное повторяющиеся проверки доступа гостевых участников группы B и однофакторная проверка доступа гостевых участников группы C, то каждое из этих повторений только что запущено, и вызывающий запрос запрашивает проверки доступа с помощью шаблона бизнес-потока отзывов гостевых участников групп,  Будут возвращены три объекта, представляющие три ряда, а также три объекта для текущих экземпляров проверки доступа и, возможно, три объекта для следующих будущих экземпляров. Чтобы получить экземпляры повторяющейся проверки доступа или экземпляр проверки доступа, запланированный на определенный месяц или квартал, вызывающий объект может впоследствии перемещаться по  связи экземпляра повторяющегося **объекта accessReview**. Связь **экземпляра** связывается с **объектами accessReview** для текущего или прошлых экземпляров повторяющейся проверки доступа.

Если фильтру соответствует множество проверок доступа, чтобы повысить эффективность и избежать времени ожидания, извлеките результирующий набор на страницах, `$top` включив параметр запроса с размером страницы, например 100, `$skip=0` и параметр запроса в запрос. Эти параметры можно включить, даже если вы не предполагаете, что запрос будет охватывать несколько страниц. Если результирующий набор занимает несколько страниц, Microsoft Graph `@odata.nextLink` возвращает эту страницу со свойством в ответе, содержащее URL-адрес следующей страницы результатов. При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).

**Объекты accessReview**, возвращаемые этим API, не будут включать вложенные свойства **структуры, такие** как параметры или связи.  Чтобы получить параметры проверки доступа или связи, используйте API [get accessReview](accessreview-get.md) .


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | AccessReview.Read.All, AccessReview.ReadWrite.Membership |

 Пользователь, выполнив вход, также должен иметь роль каталога, которая позволяет ему читать проверку доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не предоставляйте текст запроса.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и массив объектов [accessReview](../resources/accessreview.md) в тексте отклика.

## <a name="examples"></a>Примеры
##### <a name="request"></a>Запрос
В следующем примере показан запрос на получение всех разных и повторяющихся проверок доступа для шаблона бизнес-потока "6e4f3d20-c5c3-407f-9695-8460952bcc68".

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviews-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-accessreviews-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>См. также

- [Получение accessReview](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


