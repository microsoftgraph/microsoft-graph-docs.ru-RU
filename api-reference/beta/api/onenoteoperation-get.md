---
title: Получение onenoteOperation
description: 'Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
ms.openlocfilehash: abd11846cce1eab5e51ffc966d754a8a47f005bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080817"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="71480-104">Получение onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="71480-104">Get onenoteOperation</span></span>

> <span data-ttu-id="71480-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71480-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71480-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71480-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71480-p103">Получение сведений о состоянии операции OneNote, выполняющейся в течение длительного времени. Применяется к операциям, возвращающим заголовок **Operation-Location** в отклике, например `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="71480-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="71480-109">Вы можете опрашивать конечную точку Operation-Location, пока свойство `status` не возвратит значение `completed` или `failed`.</span><span class="sxs-lookup"><span data-stu-id="71480-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="71480-110">Если операция имеет состояние `completed`, свойство `resourceLocation` содержит URI конечной точки ресурса.</span><span class="sxs-lookup"><span data-stu-id="71480-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="71480-111">Если состояние `failed`, свойства `@api.diagnostics` и error предоставляют данные об ошибке.</span><span class="sxs-lookup"><span data-stu-id="71480-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="71480-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71480-112">Permissions</span></span>
<span data-ttu-id="71480-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71480-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71480-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71480-115">Permission type</span></span>      | <span data-ttu-id="71480-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71480-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71480-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71480-117">Delegated (work or school account)</span></span> | <span data-ttu-id="71480-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71480-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="71480-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71480-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71480-120">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71480-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="71480-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71480-121">Application</span></span> | <span data-ttu-id="71480-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71480-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71480-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71480-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71480-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71480-124">Optional query parameters</span></span>
<span data-ttu-id="71480-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="71480-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71480-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71480-126">Request headers</span></span>
| <span data-ttu-id="71480-127">Имя</span><span class="sxs-lookup"><span data-stu-id="71480-127">Name</span></span>       | <span data-ttu-id="71480-128">Тип</span><span class="sxs-lookup"><span data-stu-id="71480-128">Type</span></span> | <span data-ttu-id="71480-129">Описание</span><span class="sxs-lookup"><span data-stu-id="71480-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71480-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="71480-130">Authorization</span></span>  | <span data-ttu-id="71480-131">string</span><span class="sxs-lookup"><span data-stu-id="71480-131">string</span></span>  | <span data-ttu-id="71480-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71480-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71480-134">Accept</span><span class="sxs-lookup"><span data-stu-id="71480-134">Accept</span></span> | <span data-ttu-id="71480-135">строка</span><span class="sxs-lookup"><span data-stu-id="71480-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="71480-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71480-136">Request body</span></span>
<span data-ttu-id="71480-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71480-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71480-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71480-138">Response</span></span>

<span data-ttu-id="71480-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [onenoteOperation](../resources/onenoteoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71480-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71480-140">Пример</span><span class="sxs-lookup"><span data-stu-id="71480-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71480-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="71480-141">Request</span></span>
<span data-ttu-id="71480-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71480-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="71480-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="71480-143">Response</span></span>
<span data-ttu-id="71480-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="71480-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
