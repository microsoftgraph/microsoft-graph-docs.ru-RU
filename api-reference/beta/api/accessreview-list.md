---
title: Список Акцессревиевс
description: Получение объектов Акцессревиев для Бусинессфловтемплате.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1e138f7b255053797bc671adcad7ce20ed99480
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119531"
---
# <a name="list-accessreviews"></a><span data-ttu-id="0dc80-103">Список Акцессревиевс</span><span class="sxs-lookup"><span data-stu-id="0dc80-103">List accessReviews</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dc80-104">Получение объектов [акцессревиев](../resources/accessreview.md) для определенного [бусинессфловтемплате](../resources/businessflowtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0dc80-104">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="0dc80-105">Список из нуля или более объектов **акцессревиев** возвращается для каждой одноразовой и повторяющейся проверки доступа, созданной с помощью этого шаблона бизнес-процесса.</span><span class="sxs-lookup"><span data-stu-id="0dc80-105">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="0dc80-106">Обратите внимание, что идентификаторы шаблонов бизнес-процесса чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="0dc80-106">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="0dc80-107">Если какой-либо из проверок доступа, соответствующих фильтру, является повторяющейся проверкой доступа, возвращается один объект **акцессревиев** для представления каждого повторяющегося ряда в целом.</span><span class="sxs-lookup"><span data-stu-id="0dc80-107">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole.</span></span> <span data-ttu-id="0dc80-108">Например, если имеется ежемесячная проверка доступа участников группы "гость", то есть Ежеквартальная проверка доступа участников группы "гость" для группы "б" и одноразовый доступ к просмотру гостевых участников группы C и вызывающим запросом на рецензию доступа с бизнес-процессом шаблон рецензирования участников группы, будут возвращены три объекта.</span><span class="sxs-lookup"><span data-stu-id="0dc80-108">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned.</span></span> <span data-ttu-id="0dc80-109">Чтобы получить экземпляры повторяющейся проверки доступа или экземпляра проверки доступа, запланированный на определенный месяц или квартал, вызывающий может впоследствии перемещаться по связи **экземпляра** объекта повторяющегося объекта **акцессревиев** .</span><span class="sxs-lookup"><span data-stu-id="0dc80-109">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="0dc80-110">Связь **экземпляра** связывается с объектами **акцессревиев** для текущего или прошлых экземпляров проверки поповторяющегося доступа.</span><span class="sxs-lookup"><span data-stu-id="0dc80-110">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="0dc80-111">Если в соответствии с фильтром все обзоры доступа совпадают, чтобы повысить эффективность и избежать истечения времени ожидания, извлеките набор результатов на `$top` страницы, указав для параметра запроса размер страницы, например 100, и `$skip=0` параметр запроса в запросе.</span><span class="sxs-lookup"><span data-stu-id="0dc80-111">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="0dc80-112">Эти параметры можно включить, даже если не предполагается, что запрос будет охватывать несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="0dc80-112">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="0dc80-113">Когда набор результатов охватывает несколько страниц, Microsoft Graph возвращает эту страницу со `@odata.nextLink` свойством в ответе, который содержит URL-адрес следующей страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="0dc80-113">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="0dc80-114">При наличии этого свойства Продолжайте делать дополнительные запросы с `@odata.nextLink` URL-адресом в каждом ответе до тех пор, пока не будут возвращены все результаты, как описано в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="0dc80-114">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="0dc80-115">Объекты **акцессревиев** , возвращаемые этим API, не будут содержать вложенные свойства структуры, такие как **Параметры**или связи.</span><span class="sxs-lookup"><span data-stu-id="0dc80-115">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="0dc80-116">Чтобы получить параметры или связи проверки доступа, используйте API [Get акцессревиев](accessreview-get.md) .</span><span class="sxs-lookup"><span data-stu-id="0dc80-116">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="0dc80-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dc80-117">Permissions</span></span>
<span data-ttu-id="0dc80-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dc80-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dc80-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dc80-120">Permission type</span></span>                        | <span data-ttu-id="0dc80-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dc80-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dc80-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dc80-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dc80-123">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0dc80-123">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0dc80-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dc80-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dc80-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dc80-125">Not supported.</span></span> |
|<span data-ttu-id="0dc80-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="0dc80-126">Application</span></span>                            | <span data-ttu-id="0dc80-127">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="0dc80-127">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="0dc80-128">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="0dc80-128">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="0dc80-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dc80-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="0dc80-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dc80-130">Request headers</span></span>
| <span data-ttu-id="0dc80-131">Имя</span><span class="sxs-lookup"><span data-stu-id="0dc80-131">Name</span></span>         | <span data-ttu-id="0dc80-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0dc80-132">Type</span></span>        | <span data-ttu-id="0dc80-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0dc80-133">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0dc80-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dc80-134">Authorization</span></span> | <span data-ttu-id="0dc80-135">string</span><span class="sxs-lookup"><span data-stu-id="0dc80-135">string</span></span> | <span data-ttu-id="0dc80-p106">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dc80-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dc80-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0dc80-138">Request body</span></span>
<span data-ttu-id="0dc80-139">Не указывайте текст запроса.</span><span class="sxs-lookup"><span data-stu-id="0dc80-139">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0dc80-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dc80-140">Response</span></span>
<span data-ttu-id="0dc80-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и массив объектов [акцессревиев](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0dc80-141">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0dc80-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="0dc80-142">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="0dc80-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dc80-143">Request</span></span>
<span data-ttu-id="0dc80-144">В приведенном ниже примере показан запрос на получение всех одноразовых и повторяющихся проверок доступа для шаблона рабочего процесса "6e4f3d20-c5c3-407f-9695-8460952bcc68".</span><span class="sxs-lookup"><span data-stu-id="0dc80-144">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0dc80-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dc80-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0dc80-146">C#</span><span class="sxs-lookup"><span data-stu-id="0dc80-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0dc80-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dc80-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0dc80-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dc80-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---
null
---


##### <a name="response"></a><span data-ttu-id="0dc80-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dc80-149">Response</span></span>
><span data-ttu-id="0dc80-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0dc80-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0dc80-152">См. также</span><span class="sxs-lookup"><span data-stu-id="0dc80-152">See also</span></span>

- [<span data-ttu-id="0dc80-153">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="0dc80-153">Get accessReview</span></span>](accessreview-get.md)


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
