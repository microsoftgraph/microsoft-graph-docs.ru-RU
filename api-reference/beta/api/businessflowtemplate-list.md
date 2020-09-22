---
title: Список Бусинессфловтемплатес
description: В функции проверок доступа Azure AD перечислите все объекты Бусинессфловтемплате.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: adfa33bda915fcc74e234ab7473d62a761716d05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987723"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="01ea9-103">Список Бусинессфловтемплатес</span><span class="sxs-lookup"><span data-stu-id="01ea9-103">List businessFlowTemplates</span></span>

<span data-ttu-id="01ea9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01ea9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01ea9-105">В функции [проверок доступа](../resources/accessreviews-root.md) Azure AD перечислите все объекты [бусинессфловтемплате](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="01ea9-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="01ea9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01ea9-106">Permissions</span></span>
<span data-ttu-id="01ea9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01ea9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01ea9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01ea9-109">Permission type</span></span>                        | <span data-ttu-id="01ea9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01ea9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="01ea9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01ea9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01ea9-112">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="01ea9-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="01ea9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01ea9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01ea9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01ea9-114">Not supported.</span></span> |
|<span data-ttu-id="01ea9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01ea9-115">Application</span></span>                            | <span data-ttu-id="01ea9-116">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="01ea9-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="01ea9-117">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="01ea9-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="01ea9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01ea9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="01ea9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01ea9-119">Request headers</span></span>
| <span data-ttu-id="01ea9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="01ea9-120">Name</span></span>         | <span data-ttu-id="01ea9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="01ea9-121">Type</span></span>        | <span data-ttu-id="01ea9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="01ea9-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="01ea9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01ea9-123">Authorization</span></span> | <span data-ttu-id="01ea9-124">string</span><span class="sxs-lookup"><span data-stu-id="01ea9-124">string</span></span> | <span data-ttu-id="01ea9-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01ea9-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01ea9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01ea9-127">Request body</span></span>
<span data-ttu-id="01ea9-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="01ea9-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="01ea9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ea9-129">Response</span></span>
<span data-ttu-id="01ea9-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [бусинессфловтемплате](../resources/businessflowtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01ea9-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01ea9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="01ea9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01ea9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="01ea9-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01ea9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="01ea9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="01ea9-134">C#</span><span class="sxs-lookup"><span data-stu-id="01ea9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01ea9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01ea9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01ea9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01ea9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="01ea9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="01ea9-137">Response</span></span>
><span data-ttu-id="01ea9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01ea9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="01ea9-140">См. также</span><span class="sxs-lookup"><span data-stu-id="01ea9-140">See also</span></span>

| <span data-ttu-id="01ea9-141">Метод</span><span class="sxs-lookup"><span data-stu-id="01ea9-141">Method</span></span>           | <span data-ttu-id="01ea9-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01ea9-142">Return Type</span></span>    |<span data-ttu-id="01ea9-143">Описание</span><span class="sxs-lookup"><span data-stu-id="01ea9-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01ea9-144">Создание Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="01ea9-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="01ea9-145">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="01ea9-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="01ea9-146">Создание нового Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="01ea9-146">Create a new accessReview.</span></span> |




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


