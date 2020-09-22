---
title: Список Акцессревиевс
description: Получение объектов Акцессревиев для Бусинессфловтемплате.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d84f6315e2a2ca3a82d167cfc3d1137d861aec8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983574"
---
# <a name="list-accessreviews"></a>Список Акцессревиевс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объектов [акцессревиев](../resources/accessreview.md) для определенного [бусинессфловтемплате](../resources/businessflowtemplate.md). Список из нуля или более объектов **акцессревиев** возвращается для каждой одноразовой и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-процесса.  Обратите внимание, что идентификаторы шаблонов бизнес-процесса чувствительны к регистру.

>[!NOTE]
> Если какой-либо из проверок доступа, соответствующих фильтру, является повторяющейся проверкой доступа, один объект **акцессревиев** будет возвращен для представления каждого повторяющегося ряда в целом, в дополнение к любому текущему, предшествующему и следующему экземпляру. Например, если имеется месячная проверка доступа участников группы "гость", "Ежеквартальная проверка доступа" участников "гость" группы "б" и "однократный доступ" участников группы C, то каждый из этих повторений начался только что начался, а вызывающие запросы на проверку доступа с помощью шаблона бизнес-процесса, рассматривающего участников групп. будут возвращены три объекта, представляющие три ряда, а также три объекта для текущих экземпляров проверки доступа, и потенциально три объекта для следующих последующих экземпляров. Чтобы получить экземпляры повторяющейся проверки доступа или экземпляра проверки доступа, запланированный на определенный месяц или квартал, вызывающий может впоследствии перемещаться по связи **экземпляра** объекта повторяющегося объекта **акцессревиев** . Связь **экземпляра** связывается с объектами **акцессревиев** для текущего или прошлых экземпляров проверки поповторяющегося доступа.

Если в соответствии с фильтром все обзоры доступа совпадают, чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на страницы, указав `$top` для параметра запроса размер страницы, например 100, и `$skip=0` параметр запроса в запросе. Эти параметры можно включить, даже если не предполагается, что запрос будет охватывать несколько страниц. Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу со `@odata.nextLink` свойством в ответе, который содержит URL-адрес следующей страницы результатов. При наличии этого свойства Продолжайте делать дополнительные запросы с `@odata.nextLink` URL-адресом в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging.md).

Объекты **акцессревиев** , возвращаемые этим API, не будут содержать вложенные свойства структуры, такие как **Параметры**или связи.  Чтобы получить параметры или связи проверки доступа, используйте API [Get акцессревиев](accessreview-get.md) .


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership |

 Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Тип        | Описание |
|:-------------|:------------|:------------|
| Authorization | string | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиев](../resources/accessreview.md) в тексте отклика.

## <a name="examples"></a>Примеры
##### <a name="request"></a>Запрос
В приведенном ниже примере показан запрос на получение всех одноразовых и повторяющихся проверок доступа для шаблона рабочего процесса "6e4f3d20-c5c3-407f-9695-8460952bcc68".

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

---



---


##### <a name="response"></a>Отклик
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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

- [Получение Акцессревиев](accessreview-get.md)


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


