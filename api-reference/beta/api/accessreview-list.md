---
title: AccessReviews списка
description: Извлечение объектов accessReview для businessFlowTemplate.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 443ffc2c5a31ac33cba89cb689884a3bae4ab645
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048493"
---
# <a name="list-accessreviews"></a><span data-ttu-id="9be98-103">AccessReviews списка</span><span class="sxs-lookup"><span data-stu-id="9be98-103">List accessReviews</span></span>

<span data-ttu-id="9be98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9be98-105">Извлечение [объектов accessReview](../resources/accessreview.md) для определенного [businessFlowTemplate.](../resources/businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="9be98-105">Retrieve the [accessReview](../resources/accessreview.md) objects for a particular [businessFlowTemplate](../resources/businessflowtemplate.md).</span></span> <span data-ttu-id="9be98-106">Возвращается список объектов **accessReview** с нулем или более для каждого разового и повторяющегося обзора доступа, созданного с помощью этого шаблона бизнес-потока.</span><span class="sxs-lookup"><span data-stu-id="9be98-106">A list of zero or more **accessReview** objects are returned, for each one-time and recurring access review that was created with that business flow template.</span></span>  <span data-ttu-id="9be98-107">Обратите внимание, что ID-данные шаблона бизнес-потока чувствительны к делу.</span><span class="sxs-lookup"><span data-stu-id="9be98-107">Note that business flow template IDs are case sensitive.</span></span>

>[!NOTE]
> <span data-ttu-id="9be98-108">Если любой из отзывов доступа, которые соответствуют фильтру, представляет собой повторяющиеся обзоры доступа, будет возвращен один объект **accessReview,** который будет представлять каждую повторяющуюся серию в целом, в дополнение к любому текущему, прошлому и следующему экземпляру.</span><span class="sxs-lookup"><span data-stu-id="9be98-108">If any of the access reviews that match the filter is a recurring access review, one **accessReview** object will be returned to represent each recurring series as a whole, in addition to any current, past and the next upcoming instance.</span></span> <span data-ttu-id="9be98-109">Например, если имеется ежемесячный повторяющийся обзор доступа гостевых членов группы A, ежекварточный повторяющийся обзор доступа гостевых членов группы B и разовая проверка доступа гостевых членов группы C, каждый из этих повторений только начался, и вызывающий запросы для отзывов доступа с шаблоном бизнес-потока отзывов приглашенных членов групп будут возвращены три объекта, представляющие три серии, а также три объекта для текущих экземпляров обзора доступа и, возможно, три объекта для следующих экземпляров.</span><span class="sxs-lookup"><span data-stu-id="9be98-109">For example, if there is a monthly recurring access review of guest members of group A, a quarterly recurring access review of guest members of group B, and a one-time access review of guest members of group C, each of these recurrences have just started, and the caller queries for access reviews with a business flow template of reviews of guest members of groups, three objects will be returned representing the three series, as well as three objects for the current access review instances, and potentially three objects for the next upcoming instances.</span></span> <span data-ttu-id="9be98-110">Чтобы получить экземпляры повторяемого обзора доступа или экземпляр обзора доступа, запланированный на определенный месяц  или квартал, вызывающий может впоследствии перемещаться по отношениям экземпляра повторяющегося объекта **accessReview.**</span><span class="sxs-lookup"><span data-stu-id="9be98-110">To retrieve the instances of a recurring access review, or the access review instance scheduled for a particular month or quarter, the caller can subsequently navigate the **instance** relationship of the recurring **accessReview** object.</span></span> <span data-ttu-id="9be98-111">Связь **экземпляра** со ссылками на **объекты accessReview** для текущих или прошлых экземпляров повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="9be98-111">The **instance** relationship links to the **accessReview** objects for a current or the past instances of the recurring access review.</span></span>

<span data-ttu-id="9be98-112">Если многие обзоры доступа соответствуют фильтру, чтобы повысить эффективность и избежать периодов времени, извлекайте результат, заданный на страницах, включив параметр запроса с размером страницы, например 100, и параметр запроса в `$top` `$skip=0` запросе.</span><span class="sxs-lookup"><span data-stu-id="9be98-112">If many access reviews match the filter, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the `$top` query parameter with a page size, for example 100, and the `$skip=0` query parameter in the request.</span></span> <span data-ttu-id="9be98-113">Эти параметры можно включить, даже если вы не ожидаете, что запрос будет охватывать несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="9be98-113">These parameters can be included even when you do not anticipate that the request will span multiple pages.</span></span> <span data-ttu-id="9be98-114">Если набор результатов охватывает несколько страниц, корпорация Майкрософт Graph возвращает эту страницу с свойством в ответе, содержам URL-адрес на `@odata.nextLink` следующую страницу результатов.</span><span class="sxs-lookup"><span data-stu-id="9be98-114">When a result set spans multiple pages, Microsoft Graph returns that page with an `@odata.nextLink` property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="9be98-115">При наличии этого свойства продолжайте выполнять дополнительные запросы с URL-адресом `@odata.nextLink` в каждом отклике, пока не будут возвращены все результаты, как описано в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging.md).</span><span class="sxs-lookup"><span data-stu-id="9be98-115">If that property is present, continue making additional requests with the `@odata.nextLink` URL in each response, until all the results are returned, as described in [paging Microsoft Graph data in your app](/graph/paging.md).</span></span>

<span data-ttu-id="9be98-116">Объекты **accessReview,** возвращенные этим API, не будут включать вложенные свойства структуры, такие как **параметры** или отношения.</span><span class="sxs-lookup"><span data-stu-id="9be98-116">The **accessReview** objects returned by this API will not include nested structure properties such as **settings**, or relationships.</span></span>  <span data-ttu-id="9be98-117">Чтобы получить параметры обзора доступа или отношения, используйте [API get accessReview.](accessreview-get.md)</span><span class="sxs-lookup"><span data-stu-id="9be98-117">To retrieve an access review settings or relationships, use the [get accessReview](accessreview-get.md) API.</span></span>


## <a name="permissions"></a><span data-ttu-id="9be98-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9be98-118">Permissions</span></span>
<span data-ttu-id="9be98-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9be98-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9be98-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9be98-121">Permission type</span></span>                        | <span data-ttu-id="9be98-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9be98-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be98-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9be98-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be98-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be98-124">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="9be98-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9be98-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be98-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9be98-126">Not supported.</span></span> |
|<span data-ttu-id="9be98-127">Приложение</span><span class="sxs-lookup"><span data-stu-id="9be98-127">Application</span></span>                            | <span data-ttu-id="9be98-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="9be98-128">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

 <span data-ttu-id="9be98-129">Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="9be98-129">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="9be98-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9be98-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a><span data-ttu-id="9be98-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9be98-131">Request headers</span></span>
| <span data-ttu-id="9be98-132">Имя</span><span class="sxs-lookup"><span data-stu-id="9be98-132">Name</span></span>         | <span data-ttu-id="9be98-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9be98-133">Type</span></span>        | <span data-ttu-id="9be98-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9be98-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9be98-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="9be98-135">Authorization</span></span> | <span data-ttu-id="9be98-136">string</span><span class="sxs-lookup"><span data-stu-id="9be98-136">string</span></span> | <span data-ttu-id="9be98-p106">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9be98-p106">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9be98-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9be98-139">Request body</span></span>
<span data-ttu-id="9be98-140">Не поставляем тело запроса.</span><span class="sxs-lookup"><span data-stu-id="9be98-140">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="9be98-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9be98-141">Response</span></span>
<span data-ttu-id="9be98-142">В случае успешной работы этот метод возвращает код отклика и массив `200 OK` [объектов accessReview](../resources/accessreview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9be98-142">If successful, this method returns a `200 OK` response code and an array of [accessReview](../resources/accessreview.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9be98-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="9be98-143">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="9be98-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="9be98-144">Request</span></span>
<span data-ttu-id="9be98-145">В следующем примере показан запрос на извлечение всех разных и повторяющихся обзоров доступа для шаблона бизнес-потока '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span><span class="sxs-lookup"><span data-stu-id="9be98-145">The following example shows a request to retrieve all the one-time and recurring access reviews for a business flow template '6e4f3d20-c5c3-407f-9695-8460952bcc68'.</span></span>

# <a name="http"></a>[<span data-ttu-id="9be98-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9be98-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="9be98-147">C#</span><span class="sxs-lookup"><span data-stu-id="9be98-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9be98-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9be98-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9be98-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9be98-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9be98-150">Java</span><span class="sxs-lookup"><span data-stu-id="9be98-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a><span data-ttu-id="9be98-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9be98-151">Response</span></span>
><span data-ttu-id="9be98-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9be98-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9be98-153">См. также</span><span class="sxs-lookup"><span data-stu-id="9be98-153">See also</span></span>

- [<span data-ttu-id="9be98-154">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="9be98-154">Get accessReview</span></span>](accessreview-get.md)


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


