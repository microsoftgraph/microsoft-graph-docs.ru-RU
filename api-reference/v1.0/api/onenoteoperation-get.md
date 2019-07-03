---
title: Получение onenoteOperation
description: 'Получение состояния длительной операции с OneNote. Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ae44a94114c7ed85633393bfc1a9014116ed32ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457599"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="9c75a-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="9c75a-104">Get onenoteOperation</span></span>

<span data-ttu-id="9c75a-105">Получение состояния длительной операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="9c75a-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="9c75a-106">Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.</span><span class="sxs-lookup"><span data-stu-id="9c75a-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="9c75a-107">Вы можете опросить конечную точку Operations – Location `status` , пока `completed` свойство `failed`не возвратит значение или.</span><span class="sxs-lookup"><span data-stu-id="9c75a-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="9c75a-108">Если состояние имеет `completed`значение, `resourceLocation` свойство содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="9c75a-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="9c75a-109">Если состояние имеет `failed`значение, то ошибка и `@api.diagnostics` свойства предоставляют сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="9c75a-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c75a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c75a-110">Permissions</span></span>
<span data-ttu-id="9c75a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c75a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c75a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c75a-113">Permission type</span></span>      | <span data-ttu-id="9c75a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c75a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c75a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c75a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9c75a-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c75a-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c75a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c75a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c75a-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c75a-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9c75a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c75a-119">Application</span></span> | <span data-ttu-id="9c75a-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c75a-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c75a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c75a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c75a-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c75a-122">Optional query parameters</span></span>
<span data-ttu-id="9c75a-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c75a-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c75a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c75a-124">Request headers</span></span>
| <span data-ttu-id="9c75a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9c75a-125">Name</span></span>       | <span data-ttu-id="9c75a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9c75a-126">Type</span></span> | <span data-ttu-id="9c75a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9c75a-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c75a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c75a-128">Authorization</span></span>  | <span data-ttu-id="9c75a-129">string</span><span class="sxs-lookup"><span data-stu-id="9c75a-129">string</span></span>  | <span data-ttu-id="9c75a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c75a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c75a-132">Accept</span><span class="sxs-lookup"><span data-stu-id="9c75a-132">Accept</span></span> | <span data-ttu-id="9c75a-133">строка</span><span class="sxs-lookup"><span data-stu-id="9c75a-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9c75a-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c75a-134">Request body</span></span>
<span data-ttu-id="9c75a-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c75a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c75a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c75a-136">Response</span></span>

<span data-ttu-id="9c75a-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [onenoteOperation](../resources/onenoteoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c75a-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c75a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9c75a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c75a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c75a-139">Request</span></span>
<span data-ttu-id="9c75a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c75a-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9c75a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c75a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c75a-142">C#</span><span class="sxs-lookup"><span data-stu-id="9c75a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c75a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c75a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c75a-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9c75a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c75a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c75a-145">Response</span></span>
<span data-ttu-id="9c75a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c75a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
