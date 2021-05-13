---
title: Список accessReviewHistoryDefinitions
description: Получите список объектов accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 633b8e075f9bbeedf47e24fcebf560a85d2590d6
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474159"
---
# <a name="list-accessreviewhistorydefinitions"></a><span data-ttu-id="c4430-103">Список accessReviewHistoryDefinitions</span><span class="sxs-lookup"><span data-stu-id="c4430-103">List accessReviewHistoryDefinitions</span></span>
<span data-ttu-id="c4430-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4430-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4430-105">[Извлечение объектов accessReviewHistoryDefinition,](../resources/accessreviewhistorydefinition.md) созданных за последние 30 дней, включая все вложенные свойства.</span><span class="sxs-lookup"><span data-stu-id="c4430-105">Retrieve the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects created in the last 30 days, including all nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="c4430-106">Размер страницы по умолчанию для этого API — 100 **объектов accessReviewHistoryDefinitions.**</span><span class="sxs-lookup"><span data-stu-id="c4430-106">The default page size for this API is 100 **accessReviewHistoryDefinitions** objects.</span></span> <span data-ttu-id="c4430-107">Чтобы повысить эффективность и избежать периодов времени из-за больших наборов результатов, применяйте pagination с помощью `$skip` `$top` параметров запроса и запросов.</span><span class="sxs-lookup"><span data-stu-id="c4430-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="c4430-108">Дополнительные сведения см. в статье [Разбивка данных Microsoft Graph по страницам в приложении](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="c4430-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
>
><span data-ttu-id="c4430-109">Если параметры запроса не предоставлены и результатов более 100, microsoft Graph автоматически будет предоставлять результаты по 100 результатов на странице.</span><span class="sxs-lookup"><span data-stu-id="c4430-109">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4430-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4430-110">Permissions</span></span>

<span data-ttu-id="c4430-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4430-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4430-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4430-113">Permission type</span></span>|<span data-ttu-id="c4430-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4430-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4430-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4430-115">Delegated (work or school account)</span></span>|<span data-ttu-id="c4430-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4430-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="c4430-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4430-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4430-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4430-118">Not supported.</span></span>|
|<span data-ttu-id="c4430-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4430-119">Application</span></span>|<span data-ttu-id="c4430-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4430-120">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="c4430-121">Если подписанный пользователь не является участником роли глобального каталога администратора или членом роли каталога global Reader, возвращаются только определения, созданные пользователем, который был создан для подписи.</span><span class="sxs-lookup"><span data-stu-id="c4430-121">If the signed-in user is not a Global Admin directory role member or a Global Reader directory role member, only the definitions that the signed-in user created will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="c4430-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4430-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4430-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4430-123">Optional query parameters</span></span>
<span data-ttu-id="c4430-124">Этот метод поддерживает параметры `$top` `$filter` запроса OData и OData для настройки `$skip` ответа.</span><span class="sxs-lookup"><span data-stu-id="c4430-124">This method supports the `$top`, `$filter`, and `$skip` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c4430-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c4430-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c4430-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4430-126">Request headers</span></span>
|<span data-ttu-id="c4430-127">Имя</span><span class="sxs-lookup"><span data-stu-id="c4430-127">Name</span></span>|<span data-ttu-id="c4430-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c4430-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4430-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4430-129">Authorization</span></span>|<span data-ttu-id="c4430-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4430-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4430-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4430-132">Request body</span></span>
<span data-ttu-id="c4430-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4430-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4430-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4430-134">Response</span></span>

<span data-ttu-id="c4430-135">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4430-135">If successful, this method returns a `200 OK` response code and a collection of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4430-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4430-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4430-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4430-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4430-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4430-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistorydefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
```
# <a name="c"></a>[<span data-ttu-id="c4430-139">C#</span><span class="sxs-lookup"><span data-stu-id="c4430-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4430-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4430-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4430-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4430-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4430-142">Java</span><span class="sxs-lookup"><span data-stu-id="c4430-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4430-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4430-143">Response</span></span>
><span data-ttu-id="c4430-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4430-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "isCollection": "true"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.count": 1,
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
      "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
      "displayName": "Last quarter's group reviews April 2021",
      "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
      "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
      "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
      ],
      "status": "done",
      "createdDateTime": "2021-04-14T00:22:48.9392594Z",
      "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
      "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
      "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
      },
      "scopes": [
        {
          "@odata.type": "#microsoft.graph.accessReviewQueryScope",
          "queryType": "MicrosoftGraph",     
          "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
          "queryRoot": null
        },  
        {
          "@odata.type": "#microsoft.graph.accessReviewQueryScope",
          "queryType": "MicrosoftGraph",     
          "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
          "queryRoot": null
        }
      ]
    }
  ]
}
```
