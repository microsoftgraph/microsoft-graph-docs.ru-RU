---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
ms.openlocfilehash: a9c623eedc34c7c4d7901a0a03ed81d070eb0af7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438953"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="8ce86-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="8ce86-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce86-104">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="8ce86-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ce86-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce86-105">Permissions</span></span>
<span data-ttu-id="8ce86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ce86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ce86-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce86-108">Permission type</span></span>                        | <span data-ttu-id="8ce86-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ce86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ce86-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ce86-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ce86-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8ce86-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="8ce86-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ce86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ce86-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce86-113">Not supported.</span></span> |
|<span data-ttu-id="8ce86-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ce86-114">Application</span></span>                            | <span data-ttu-id="8ce86-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ce86-115">AccessReview.Read.All</span></span> |

<span data-ttu-id="8ce86-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="8ce86-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ce86-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ce86-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="8ce86-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ce86-118">Request headers</span></span>
| <span data-ttu-id="8ce86-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8ce86-119">Name</span></span>         | <span data-ttu-id="8ce86-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8ce86-120">Type</span></span>        | <span data-ttu-id="8ce86-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce86-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8ce86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ce86-122">Authorization</span></span> | <span data-ttu-id="8ce86-123">string</span><span class="sxs-lookup"><span data-stu-id="8ce86-123">string</span></span> | <span data-ttu-id="8ce86-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ce86-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce86-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ce86-126">Request body</span></span>
<span data-ttu-id="8ce86-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="8ce86-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="8ce86-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ce86-128">Response</span></span>
<span data-ttu-id="8ce86-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ce86-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ce86-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8ce86-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ce86-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ce86-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8ce86-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ce86-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ce86-133">C#</span><span class="sxs-lookup"><span data-stu-id="8ce86-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ce86-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ce86-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ce86-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ce86-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8ce86-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ce86-136">Response</span></span>
><span data-ttu-id="8ce86-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ce86-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8ce86-139">См. также</span><span class="sxs-lookup"><span data-stu-id="8ce86-139">See also</span></span>

| <span data-ttu-id="8ce86-140">Метод</span><span class="sxs-lookup"><span data-stu-id="8ce86-140">Method</span></span>           | <span data-ttu-id="8ce86-141">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ce86-141">Return Type</span></span>    |<span data-ttu-id="8ce86-142">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce86-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ce86-143">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8ce86-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="8ce86-144">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8ce86-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="8ce86-145">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="8ce86-145">Create a new accessReview.</span></span> |




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
