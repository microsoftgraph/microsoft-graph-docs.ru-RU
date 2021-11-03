---
title: AccessReviews списка
description: Извлечение объектов accessReview для businessFlowTemplate.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 420cf16b0f6c2e3703761ad60375bf98835a96d0
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729600"
---
# <a name="list-accessreviews"></a>AccessReviews списка

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение [объектов accessReview](../resources/accessreview.md) для определенного [businessFlowTemplate.](../resources/businessflowtemplate.md) Возвращается список объектов **accessReview** с нулем или более для каждого разового и повторяющегося обзора доступа, созданного с помощью этого шаблона бизнес-потока.  Обратите внимание, что ID-данные шаблона бизнес-потока чувствительны к делу.

>[!NOTE]
> Если любой из отзывов доступа, которые соответствуют фильтру, представляет собой повторяющиеся обзоры доступа, будет возвращен один объект **accessReview,** который будет представлять каждую повторяющуюся серию в целом, в дополнение к любому текущему, прошлому и следующему экземпляру. Например, если имеется ежемесячный повторяющийся обзор доступа гостевых членов группы A, ежекварточный повторяющийся обзор доступа гостевых членов группы B и разовая проверка доступа гостей группы C, каждое из этих повторений только началось, и вызывающий запросы на отзывы о доступе с шаблоном бизнес-потока отзывов приглашенных членов групп,  Будут возвращены три объекта, представляющие три серии, а также три объекта для текущих экземпляров обзора доступа и потенциально три объекта для следующих экземпляров. Чтобы получить экземпляры повторяемого обзора доступа или экземпляр обзора доступа, запланированный на определенный месяц  или квартал, вызывающий может впоследствии перемещаться по отношениям экземпляра повторяющегося объекта **accessReview.** Связь **экземпляра** со ссылками на **объекты accessReview** для текущих или прошлых экземпляров повторного обзора доступа.

Если многие обзоры доступа соответствуют фильтру, чтобы повысить эффективность и избежать периодов времени, извлекайте результат, заданный на страницах, включив параметр запроса с размером страницы, например 100, и параметр запроса в `$top` `$skip=0` запросе. Эти параметры можно включить, даже если вы не ожидаете, что запрос будет охватывать несколько страниц. Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством в ответе, содержам URL-адрес на `@odata.nextLink` следующую страницу результатов. При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).

Объекты **accessReview,** возвращенные этим API, не будут включать вложенные свойства структуры, такие как **параметры** или отношения.  Чтобы получить параметры обзора доступа или отношения, используйте [API get accessReview.](accessreview-get.md)


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | AccessReview.Read.All, AccessReview.ReadWrite.Membership |

 Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Основной текст запроса
Не поставляем тело запроса.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReview](../resources/accessreview.md) в тексте отклика.

## <a name="examples"></a>Примеры
##### <a name="request"></a>Запрос
В следующем примере показан запрос на извлечение всех разных и повторяющихся обзоров доступа для шаблона бизнес-потока '6e4f3d20-c5c3-407f-9695-8460952bcc68'.

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

- [Получить accessReview](accessreview-get.md)


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


