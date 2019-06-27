---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
ms.openlocfilehash: 3f7fc6ac155b22845c13c75fddd1af49f7b32e32
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262449"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="0da77-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="0da77-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0da77-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="0da77-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0da77-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0da77-105">Permissions</span></span>
<span data-ttu-id="0da77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da77-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0da77-108">Permission type</span></span>                        | <span data-ttu-id="0da77-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0da77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da77-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0da77-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0da77-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0da77-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0da77-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0da77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da77-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0da77-113">Not supported.</span></span> |
|<span data-ttu-id="0da77-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0da77-114">Application</span></span>                            | <span data-ttu-id="0da77-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="0da77-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="0da77-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="0da77-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="0da77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0da77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="0da77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0da77-118">Request headers</span></span>
| <span data-ttu-id="0da77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0da77-119">Name</span></span>         | <span data-ttu-id="0da77-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0da77-120">Type</span></span>        | <span data-ttu-id="0da77-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0da77-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0da77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0da77-122">Authorization</span></span> | <span data-ttu-id="0da77-123">string</span><span class="sxs-lookup"><span data-stu-id="0da77-123">string</span></span> | <span data-ttu-id="0da77-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0da77-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0da77-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0da77-126">Request body</span></span>
<span data-ttu-id="0da77-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="0da77-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0da77-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0da77-128">Response</span></span>
<span data-ttu-id="0da77-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0da77-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0da77-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0da77-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0da77-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0da77-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="0da77-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0da77-132">Response</span></span>
><span data-ttu-id="0da77-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0da77-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0da77-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0da77-135">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0da77-136">C#</span><span class="sxs-lookup"><span data-stu-id="0da77-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0da77-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="0da77-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0da77-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0da77-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_businessFlowTemplate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="0da77-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0da77-139">See also</span></span>

| <span data-ttu-id="0da77-140">Метод</span><span class="sxs-lookup"><span data-stu-id="0da77-140">Method</span></span>           | <span data-ttu-id="0da77-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0da77-141">Return Type</span></span>    |<span data-ttu-id="0da77-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0da77-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0da77-143">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="0da77-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="0da77-144">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="0da77-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="0da77-145">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="0da77-145">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}
-->
