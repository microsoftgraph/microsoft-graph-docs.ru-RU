---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c5d3ae6cdb761ea54d30b7821284fb0c2efa7b9b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173022"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="2b53d-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="2b53d-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b53d-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="2b53d-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b53d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b53d-105">Permissions</span></span>
<span data-ttu-id="2b53d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b53d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b53d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b53d-108">Permission type</span></span>                        | <span data-ttu-id="2b53d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b53d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b53d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b53d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b53d-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b53d-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="2b53d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b53d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b53d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b53d-113">Not supported.</span></span> |
|<span data-ttu-id="2b53d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b53d-114">Application</span></span>                            | <span data-ttu-id="2b53d-115">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="2b53d-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="2b53d-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="2b53d-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b53d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b53d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="2b53d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b53d-118">Request headers</span></span>
| <span data-ttu-id="2b53d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2b53d-119">Name</span></span>         | <span data-ttu-id="2b53d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2b53d-120">Type</span></span>        | <span data-ttu-id="2b53d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2b53d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2b53d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b53d-122">Authorization</span></span> | <span data-ttu-id="2b53d-123">string</span><span class="sxs-lookup"><span data-stu-id="2b53d-123">string</span></span> | <span data-ttu-id="2b53d-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b53d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b53d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b53d-126">Request body</span></span>
<span data-ttu-id="2b53d-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="2b53d-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="2b53d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b53d-128">Response</span></span>
<span data-ttu-id="2b53d-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b53d-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b53d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2b53d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b53d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b53d-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b53d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b53d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b53d-133">C#</span><span class="sxs-lookup"><span data-stu-id="2b53d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b53d-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b53d-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b53d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2b53d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2b53d-136">Java</span><span class="sxs-lookup"><span data-stu-id="2b53d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b53d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b53d-137">Response</span></span>
><span data-ttu-id="2b53d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b53d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="2b53d-140">См. также</span><span class="sxs-lookup"><span data-stu-id="2b53d-140">See also</span></span>

| <span data-ttu-id="2b53d-141">Метод</span><span class="sxs-lookup"><span data-stu-id="2b53d-141">Method</span></span>           | <span data-ttu-id="2b53d-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b53d-142">Return Type</span></span>    |<span data-ttu-id="2b53d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="2b53d-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b53d-144">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2b53d-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="2b53d-145">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2b53d-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="2b53d-146">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2b53d-146">Create a new accessReview.</span></span> |




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
