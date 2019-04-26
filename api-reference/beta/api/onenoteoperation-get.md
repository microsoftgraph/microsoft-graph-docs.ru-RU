---
title: Получение onenoteOperation
description: 'Получение состояния длительной операции с OneNote. Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 6d9e880a63eef7290c6fad06ef53960015101f3d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338147"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="58eb1-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="58eb1-104">Get onenoteOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58eb1-105">Получение состояния длительной операции с OneNote.</span><span class="sxs-lookup"><span data-stu-id="58eb1-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="58eb1-106">Это относится к операциям, которые возвращают заголовок **operationing — Location** в ответе `CopyNotebook`, `CopyToNotebook`например `CopyToSectionGroup`, `and CopyToSection`,,.</span><span class="sxs-lookup"><span data-stu-id="58eb1-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="58eb1-107">Вы можете опросить конечную точку Operations – Location `status` , пока `completed` свойство `failed`не возвратит значение или.</span><span class="sxs-lookup"><span data-stu-id="58eb1-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="58eb1-108">Если состояние имеет `completed`значение, `resourceLocation` свойство содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="58eb1-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="58eb1-109">Если состояние имеет `failed`значение, то ошибка и `@api.diagnostics` свойства предоставляют сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="58eb1-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="58eb1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58eb1-110">Permissions</span></span>
<span data-ttu-id="58eb1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58eb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58eb1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58eb1-113">Permission type</span></span>      | <span data-ttu-id="58eb1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58eb1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58eb1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58eb1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="58eb1-116">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="58eb1-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="58eb1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58eb1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58eb1-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58eb1-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="58eb1-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58eb1-119">Application</span></span> | <span data-ttu-id="58eb1-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58eb1-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58eb1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58eb1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58eb1-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58eb1-122">Optional query parameters</span></span>
<span data-ttu-id="58eb1-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58eb1-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58eb1-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58eb1-124">Request headers</span></span>
| <span data-ttu-id="58eb1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="58eb1-125">Name</span></span>       | <span data-ttu-id="58eb1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="58eb1-126">Type</span></span> | <span data-ttu-id="58eb1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="58eb1-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="58eb1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="58eb1-128">Authorization</span></span>  | <span data-ttu-id="58eb1-129">string</span><span class="sxs-lookup"><span data-stu-id="58eb1-129">string</span></span>  | <span data-ttu-id="58eb1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58eb1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="58eb1-132">Accept</span><span class="sxs-lookup"><span data-stu-id="58eb1-132">Accept</span></span> | <span data-ttu-id="58eb1-133">string</span><span class="sxs-lookup"><span data-stu-id="58eb1-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="58eb1-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58eb1-134">Request body</span></span>
<span data-ttu-id="58eb1-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58eb1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58eb1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="58eb1-136">Response</span></span>

<span data-ttu-id="58eb1-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [onenoteOperation](../resources/onenoteoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58eb1-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58eb1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="58eb1-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58eb1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="58eb1-139">Request</span></span>
<span data-ttu-id="58eb1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58eb1-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="58eb1-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="58eb1-141">Response</span></span>
<span data-ttu-id="58eb1-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58eb1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
