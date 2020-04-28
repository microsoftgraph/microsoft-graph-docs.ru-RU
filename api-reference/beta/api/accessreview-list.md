---
title: Список Акцессревиевс
description: Получение объектов Акцессревиев для Бусинессфловтемплате.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1db57c17f1496e32bd0fb6f6ac73cb25e793f3f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441900"
---
# <a name="list-accessreviews"></a><span data-ttu-id="a6c4d-103">Список Акцессревиевс</span><span class="sxs-lookup"><span data-stu-id="a6c4d-103">List accessReviews</span></span>

<span data-ttu-id="a6c4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6c4d-105">Получение объектов [акцессревиев](../resources/accessreview.md) для определенного [бусинессфловтемплате](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a6c4d-105">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="a6c4d-106">Список из нуля или более объектов **акцессревиев** возвращается для каждой одноразовой и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-106">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="a6c4d-107">Обратите внимание, что идентификаторы шаблонов бизнес-процесса чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-107">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="a6c4d-108">Если какой-либо из проверок доступа, соответствующих фильтру, является повторяющейся проверкой доступа, один объект **акцессревиев** будет возвращен для представления каждого повторяющегося ряда в целом, в дополнение к любому текущему, предшествующему и следующему экземпляру.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-108">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole, in addition to any current, past and the next upcoming instance.</span></span> <span data-ttu-id="a6c4d-109">Например, если имеется месячная проверка доступа участников группы "гость", "Ежеквартальная проверка доступа" участников "гость" группы "б" и "однократный доступ" участников группы C, то каждый из этих повторений начался только что начался, а вызывающие запросы на проверку доступа с помощью шаблона бизнес-процесса, рассматривающего участников групп. будут возвращены три объекта, представляющие три ряда, а также три объекта для текущих экземпляров проверки доступа, и потенциально три объекта для следующих последующих экземпляров.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-109">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, each of these recurrences have just started, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned representing the three series, as well as three objects for the current access review instances, and potentially three objects for the next upcoming instances.</span></span> <span data-ttu-id="a6c4d-110">Чтобы получить экземпляры повторяющейся проверки доступа или экземпляра проверки доступа, запланированный на определенный месяц или квартал, вызывающий может впоследствии перемещаться по связи **экземпляра** объекта повторяющегося объекта **акцессревиев** .</span><span class="sxs-lookup"><span data-stu-id="a6c4d-110">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="a6c4d-111">Связь **экземпляра** связывается с объектами **акцессревиев** для текущего или прошлых экземпляров проверки поповторяющегося доступа.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-111">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="a6c4d-112">Если в соответствии с фильтром все обзоры доступа совпадают, чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на `$top` страницы, указав для параметра запроса размер страницы, например 100, и `$skip=0` параметр запроса в запросе.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-112">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="a6c4d-113">Эти параметры можно включить, даже если не предполагается, что запрос будет охватывать несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-113">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="a6c4d-114">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу со `@odata.nextLink` свойством в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-114">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="a6c4d-115">При наличии этого свойства Продолжайте делать дополнительные запросы с `@odata.nextLink` URL-адресом в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="a6c4d-115">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="a6c4d-116">Объекты **акцессревиев** , возвращаемые этим API, не будут содержать вложенные свойства структуры, такие как **Параметры**или связи.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-116">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="a6c4d-117">Чтобы получить параметры или связи проверки доступа, используйте API [Get акцессревиев](accessreview-get.md) .</span><span class="sxs-lookup"><span data-stu-id="a6c4d-117">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="a6c4d-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c4d-118">Permissions</span></span>
<span data-ttu-id="a6c4d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c4d-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c4d-121">Permission type</span></span>                        | <span data-ttu-id="a6c4d-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6c4d-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c4d-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6c4d-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6c4d-124">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a6c4d-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="a6c4d-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6c4d-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c4d-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-126">Not supported.</span></span> |
|<span data-ttu-id="a6c4d-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6c4d-127">Application</span></span>                            | <span data-ttu-id="a6c4d-128">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="a6c4d-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="a6c4d-129">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-129">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="a6c4d-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6c4d-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="a6c4d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6c4d-131">Request headers</span></span>
| <span data-ttu-id="a6c4d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="a6c4d-132">Name</span></span>         | <span data-ttu-id="a6c4d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c4d-133">Type</span></span>        | <span data-ttu-id="a6c4d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c4d-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a6c4d-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c4d-135">Authorization</span></span> | <span data-ttu-id="a6c4d-136">string</span><span class="sxs-lookup"><span data-stu-id="a6c4d-136">string</span></span> | <span data-ttu-id="a6c4d-p106">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c4d-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6c4d-139">Request body</span></span>
<span data-ttu-id="a6c4d-140">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-140">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="a6c4d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6c4d-141">Response</span></span>
<span data-ttu-id="a6c4d-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-142">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6c4d-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6c4d-143">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="a6c4d-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6c4d-144">Request</span></span>
<span data-ttu-id="a6c4d-145">В приведенном ниже примере показан запрос на получение всех одноразовых и повторяющихся проверок доступа для шаблона рабочего процесса "6e4f3d20-c5c3-407f-9695-8460952bcc68".</span><span class="sxs-lookup"><span data-stu-id="a6c4d-145">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6c4d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c4d-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="a6c4d-147">C#</span><span class="sxs-lookup"><span data-stu-id="a6c4d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6c4d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6c4d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6c4d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6c4d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
null
---


##### <a name="response"></a><span data-ttu-id="a6c4d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c4d-150">Response</span></span>
><span data-ttu-id="a6c4d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6c4d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a6c4d-153">См. также</span><span class="sxs-lookup"><span data-stu-id="a6c4d-153">See also</span></span>

- [<span data-ttu-id="a6c4d-154">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a6c4d-154">Get accessReview</span></span>](accessreview-get.md)


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
