---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5a7fe7b7212a4e26dd8f0562f4a854f812cecea1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317986"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="3a77e-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="3a77e-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a77e-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="3a77e-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a77e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a77e-105">Permissions</span></span>
<span data-ttu-id="3a77e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a77e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a77e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a77e-108">Permission type</span></span>                        | <span data-ttu-id="3a77e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a77e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a77e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a77e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a77e-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3a77e-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="3a77e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a77e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a77e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a77e-113">Not supported.</span></span> |
|<span data-ttu-id="3a77e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a77e-114">Application</span></span>                            | <span data-ttu-id="3a77e-115">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="3a77e-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="3a77e-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="3a77e-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a77e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a77e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="3a77e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a77e-118">Request headers</span></span>
| <span data-ttu-id="3a77e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3a77e-119">Name</span></span>         | <span data-ttu-id="3a77e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3a77e-120">Type</span></span>        | <span data-ttu-id="3a77e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3a77e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3a77e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a77e-122">Authorization</span></span> | <span data-ttu-id="3a77e-123">string</span><span class="sxs-lookup"><span data-stu-id="3a77e-123">string</span></span> | <span data-ttu-id="3a77e-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a77e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a77e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a77e-126">Request body</span></span>
<span data-ttu-id="3a77e-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="3a77e-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3a77e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a77e-128">Response</span></span>
<span data-ttu-id="3a77e-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a77e-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a77e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3a77e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a77e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a77e-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3a77e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a77e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3a77e-133">C#</span><span class="sxs-lookup"><span data-stu-id="3a77e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a77e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a77e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3a77e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3a77e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3a77e-136">Java</span><span class="sxs-lookup"><span data-stu-id="3a77e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3a77e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a77e-137">Response</span></span>
><span data-ttu-id="3a77e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a77e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3a77e-140">См. также</span><span class="sxs-lookup"><span data-stu-id="3a77e-140">See also</span></span>

| <span data-ttu-id="3a77e-141">Метод</span><span class="sxs-lookup"><span data-stu-id="3a77e-141">Method</span></span>           | <span data-ttu-id="3a77e-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3a77e-142">Return Type</span></span>    |<span data-ttu-id="3a77e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3a77e-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a77e-144">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="3a77e-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="3a77e-145">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="3a77e-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="3a77e-146">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="3a77e-146">Create a new accessReview.</span></span> |




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
