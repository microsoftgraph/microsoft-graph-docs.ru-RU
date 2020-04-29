---
title: Получение onenoteOperation
description: 'Получение состояния длительной операции с OneNote. Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: ffb817c4c0a5ec4fd163341a3e8d0b3f905ac4c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511287"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="d029a-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="d029a-104">Get onenoteOperation</span></span>

<span data-ttu-id="d029a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d029a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d029a-106">Получение состояния длительной операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="d029a-106">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="d029a-107">Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.</span><span class="sxs-lookup"><span data-stu-id="d029a-107">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="d029a-108">Вы можете опросить конечную точку Operations – Location `status` , пока `completed` свойство `failed`не возвратит значение или.</span><span class="sxs-lookup"><span data-stu-id="d029a-108">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="d029a-109">Если состояние имеет `completed`значение, `resourceLocation` свойство содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="d029a-109">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="d029a-110">Если состояние имеет `failed`значение, то ошибка и `@api.diagnostics` свойства предоставляют сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d029a-110">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="d029a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d029a-111">Permissions</span></span>
<span data-ttu-id="d029a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d029a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d029a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d029a-114">Permission type</span></span>      | <span data-ttu-id="d029a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d029a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d029a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d029a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d029a-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d029a-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d029a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d029a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d029a-119">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d029a-119">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d029a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d029a-120">Application</span></span> | <span data-ttu-id="d029a-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d029a-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d029a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d029a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d029a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d029a-123">Optional query parameters</span></span>
<span data-ttu-id="d029a-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="d029a-124">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d029a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d029a-125">Request headers</span></span>
| <span data-ttu-id="d029a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d029a-126">Name</span></span>       | <span data-ttu-id="d029a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d029a-127">Type</span></span> | <span data-ttu-id="d029a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d029a-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d029a-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="d029a-129">Authorization</span></span>  | <span data-ttu-id="d029a-130">string</span><span class="sxs-lookup"><span data-stu-id="d029a-130">string</span></span>  | <span data-ttu-id="d029a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d029a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d029a-133">Accept</span><span class="sxs-lookup"><span data-stu-id="d029a-133">Accept</span></span> | <span data-ttu-id="d029a-134">строка</span><span class="sxs-lookup"><span data-stu-id="d029a-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d029a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d029a-135">Request body</span></span>
<span data-ttu-id="d029a-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d029a-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d029a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d029a-137">Response</span></span>

<span data-ttu-id="d029a-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [onenoteOperation](../resources/onenoteoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d029a-138">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d029a-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d029a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d029a-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d029a-140">Request</span></span>
<span data-ttu-id="d029a-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d029a-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d029a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d029a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="d029a-143">C#</span><span class="sxs-lookup"><span data-stu-id="d029a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d029a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d029a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d029a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d029a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d029a-146">Java</span><span class="sxs-lookup"><span data-stu-id="d029a-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d029a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d029a-147">Response</span></span>
<span data-ttu-id="d029a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d029a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
