---
title: Список businessFlowTemplates
description: В функции обзоров доступа Azure AD перечислите все объекты businessFlowTemplate.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 1ecb7dac1020bf243f6f58e0f6a80afc0724bfdc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437997"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="e90d3-103">Список businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="e90d3-103">List businessFlowTemplates</span></span>

<span data-ttu-id="e90d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e90d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e90d3-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) перечислите все [объекты businessFlowTemplate.](../resources/businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="e90d3-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e90d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e90d3-106">Permissions</span></span>
<span data-ttu-id="e90d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e90d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e90d3-109">Permission type</span></span>                        | <span data-ttu-id="e90d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e90d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e90d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e90d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e90d3-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e90d3-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="e90d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e90d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e90d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e90d3-114">Not supported.</span></span> |
|<span data-ttu-id="e90d3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e90d3-115">Application</span></span>                            | <span data-ttu-id="e90d3-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="e90d3-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="e90d3-117">Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="e90d3-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="e90d3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e90d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="e90d3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e90d3-119">Request headers</span></span>
| <span data-ttu-id="e90d3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e90d3-120">Name</span></span>         | <span data-ttu-id="e90d3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e90d3-121">Type</span></span>        | <span data-ttu-id="e90d3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e90d3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e90d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e90d3-123">Authorization</span></span> | <span data-ttu-id="e90d3-124">string</span><span class="sxs-lookup"><span data-stu-id="e90d3-124">string</span></span> | <span data-ttu-id="e90d3-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e90d3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e90d3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e90d3-127">Request body</span></span>
<span data-ttu-id="e90d3-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="e90d3-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e90d3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e90d3-129">Response</span></span>
<span data-ttu-id="e90d3-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [businessFlowTemplate](../resources/businessflowtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e90d3-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90d3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e90d3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e90d3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e90d3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e90d3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e90d3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="e90d3-134">C#</span><span class="sxs-lookup"><span data-stu-id="e90d3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e90d3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e90d3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e90d3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e90d3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e90d3-137">Java</span><span class="sxs-lookup"><span data-stu-id="e90d3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e90d3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e90d3-138">Response</span></span>
><span data-ttu-id="e90d3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e90d3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access reviews of guest user memberships of a group"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access reviews of guest user assignments to an application"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access reviews of assignments to an application"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access reviews of memberships of a group"
        },
        {
            "id": "d7e0b82d-997f-44d0-ac5e-de9deb087c15",
            "displayName": "Access reviews of memberships of an Azure AD role"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="e90d3-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e90d3-141">See also</span></span>

| <span data-ttu-id="e90d3-142">Метод</span><span class="sxs-lookup"><span data-stu-id="e90d3-142">Method</span></span>           | <span data-ttu-id="e90d3-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e90d3-143">Return Type</span></span>    |<span data-ttu-id="e90d3-144">Описание</span><span class="sxs-lookup"><span data-stu-id="e90d3-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e90d3-145">Создание accessReview</span><span class="sxs-lookup"><span data-stu-id="e90d3-145">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="e90d3-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="e90d3-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e90d3-147">Создание нового accessReview.</span><span class="sxs-lookup"><span data-stu-id="e90d3-147">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


