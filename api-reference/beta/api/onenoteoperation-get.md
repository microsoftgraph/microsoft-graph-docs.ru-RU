---
title: Получение onenoteOperation
description: 'Получение состояния длительной операции с OneNote. Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе, например,,, `CopyNotebook` `CopyToNotebook` `CopyToSectionGroup` `and CopyToSection` .   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 977852695d4e12eeb6d13d8c4f073e99a71cfd3a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004657"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="70858-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="70858-104">Get onenoteOperation</span></span>

<span data-ttu-id="70858-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70858-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70858-106">Получение состояния длительной операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="70858-106">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="70858-107">Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе, например,,, `CopyNotebook` `CopyToNotebook` `CopyToSectionGroup` `and CopyToSection` .</span><span class="sxs-lookup"><span data-stu-id="70858-107">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="70858-108">Вы можете опросить конечную точку Operations – Location, пока `status` свойство не возвратит значение `completed` или `failed` .</span><span class="sxs-lookup"><span data-stu-id="70858-108">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="70858-109">Если состояние имеет значение `completed` , `resourceLocation` свойство содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="70858-109">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="70858-110">Если состояние имеет значение `failed` , то ошибка и `@api.diagnostics` свойства предоставляют сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="70858-110">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="70858-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70858-111">Permissions</span></span>
<span data-ttu-id="70858-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70858-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70858-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70858-114">Permission type</span></span>      | <span data-ttu-id="70858-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70858-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70858-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70858-116">Delegated (work or school account)</span></span> | <span data-ttu-id="70858-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70858-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="70858-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70858-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70858-119">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="70858-119">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="70858-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70858-120">Application</span></span> | <span data-ttu-id="70858-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70858-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70858-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70858-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="70858-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70858-123">Optional query parameters</span></span>
<span data-ttu-id="70858-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="70858-124">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70858-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70858-125">Request headers</span></span>
| <span data-ttu-id="70858-126">Имя</span><span class="sxs-lookup"><span data-stu-id="70858-126">Name</span></span>       | <span data-ttu-id="70858-127">Тип</span><span class="sxs-lookup"><span data-stu-id="70858-127">Type</span></span> | <span data-ttu-id="70858-128">Описание</span><span class="sxs-lookup"><span data-stu-id="70858-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="70858-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="70858-129">Authorization</span></span>  | <span data-ttu-id="70858-130">string</span><span class="sxs-lookup"><span data-stu-id="70858-130">string</span></span>  | <span data-ttu-id="70858-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70858-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="70858-133">Accept</span><span class="sxs-lookup"><span data-stu-id="70858-133">Accept</span></span> | <span data-ttu-id="70858-134">строка</span><span class="sxs-lookup"><span data-stu-id="70858-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="70858-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70858-135">Request body</span></span>
<span data-ttu-id="70858-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70858-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70858-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="70858-137">Response</span></span>

<span data-ttu-id="70858-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [onenoteOperation](../resources/onenoteoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70858-138">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70858-139">Пример</span><span class="sxs-lookup"><span data-stu-id="70858-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70858-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="70858-140">Request</span></span>
<span data-ttu-id="70858-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70858-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70858-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="70858-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="70858-143">C#</span><span class="sxs-lookup"><span data-stu-id="70858-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70858-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70858-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70858-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70858-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70858-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="70858-146">Response</span></span>
<span data-ttu-id="70858-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70858-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


