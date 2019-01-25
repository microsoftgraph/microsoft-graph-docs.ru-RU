---
title: Получение onenoteOperation
description: 'Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ad9a09960c946bf41d4f62e73c65e1c7562f97ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509394"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="ba5ce-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="ba5ce-104">Get onenoteOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba5ce-p102">Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-p102">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="ba5ce-107">Вы можете опрашивать конечную точку Operation-Location, пока свойство `status` не возвратит значение `completed` или `failed`.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="ba5ce-108">Если операция имеет состояние `completed`, свойство `resourceLocation` содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="ba5ce-109">Если состояние `failed`, свойства `@api.diagnostics` и error предоставляют данные об ошибке.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba5ce-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5ce-110">Permissions</span></span>
<span data-ttu-id="ba5ce-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5ce-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5ce-113">Permission type</span></span>      | <span data-ttu-id="ba5ce-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba5ce-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba5ce-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba5ce-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ba5ce-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5ce-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba5ce-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba5ce-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba5ce-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba5ce-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ba5ce-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba5ce-119">Application</span></span> | <span data-ttu-id="ba5ce-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5ce-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba5ce-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba5ce-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba5ce-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba5ce-122">Optional query parameters</span></span>
<span data-ttu-id="ba5ce-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba5ce-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba5ce-124">Request headers</span></span>
| <span data-ttu-id="ba5ce-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ba5ce-125">Name</span></span>       | <span data-ttu-id="ba5ce-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5ce-126">Type</span></span> | <span data-ttu-id="ba5ce-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5ce-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba5ce-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba5ce-128">Authorization</span></span>  | <span data-ttu-id="ba5ce-129">string</span><span class="sxs-lookup"><span data-stu-id="ba5ce-129">string</span></span>  | <span data-ttu-id="ba5ce-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba5ce-132">Accept</span><span class="sxs-lookup"><span data-stu-id="ba5ce-132">Accept</span></span> | <span data-ttu-id="ba5ce-133">string</span><span class="sxs-lookup"><span data-stu-id="ba5ce-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ba5ce-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba5ce-134">Request body</span></span>
<span data-ttu-id="ba5ce-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba5ce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba5ce-136">Response</span></span>

<span data-ttu-id="ba5ce-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [onenoteOperation](../resources/onenoteoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba5ce-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ba5ce-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba5ce-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba5ce-139">Request</span></span>
<span data-ttu-id="ba5ce-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba5ce-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="ba5ce-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba5ce-141">Response</span></span>
<span data-ttu-id="ba5ce-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ba5ce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/onenoteoperation-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
