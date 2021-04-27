---
title: Обновление openShift
description: Обновление свойств объекта openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37d7399883980532560a7748c8082a9ff184fe1c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052084"
---
# <a name="update-openshift"></a><span data-ttu-id="a0227-103">Обновление openShift</span><span class="sxs-lookup"><span data-stu-id="a0227-103">Update openShift</span></span>

<span data-ttu-id="a0227-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0227-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0227-105">Обновление свойств объекта [openShift.](../resources/openshift.md)</span><span class="sxs-lookup"><span data-stu-id="a0227-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0227-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0227-106">Permissions</span></span>

<span data-ttu-id="a0227-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0227-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0227-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0227-109">Permission type</span></span>                        | <span data-ttu-id="a0227-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0227-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a0227-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0227-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0227-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0227-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a0227-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0227-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0227-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0227-114">Not supported.</span></span> |
| <span data-ttu-id="a0227-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0227-115">Application</span></span>                            | <span data-ttu-id="a0227-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0227-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0227-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0227-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="a0227-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0227-118">Request headers</span></span>

| <span data-ttu-id="a0227-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a0227-119">Name</span></span>       | <span data-ttu-id="a0227-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a0227-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a0227-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0227-121">Authorization</span></span> | <span data-ttu-id="a0227-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0227-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0227-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0227-124">Content-type</span></span> | <span data-ttu-id="a0227-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0227-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0227-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0227-127">Request body</span></span>

<span data-ttu-id="a0227-128">Предоставление [измененного объекта openshift](../resources/openshift.md) в теле запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0227-128">Provide the modified [openshift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="a0227-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0227-129">Property</span></span>     | <span data-ttu-id="a0227-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a0227-130">Type</span></span>        | <span data-ttu-id="a0227-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a0227-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0227-132">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="a0227-132">draftOpenShift</span></span>|<span data-ttu-id="a0227-133">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a0227-133">openShiftItem</span></span>|<span data-ttu-id="a0227-134">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="a0227-134">An unpublished open shift.</span></span>|
|<span data-ttu-id="a0227-135">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="a0227-135">schedulingGroupId</span></span>|<span data-ttu-id="a0227-136">String</span><span class="sxs-lookup"><span data-stu-id="a0227-136">String</span></span>| <span data-ttu-id="a0227-137">Scheduling group id.</span><span class="sxs-lookup"><span data-stu-id="a0227-137">Scheduling group id.</span></span> |
|<span data-ttu-id="a0227-138">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="a0227-138">sharedOpenShift</span></span>|<span data-ttu-id="a0227-139">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a0227-139">openShiftItem</span></span>|<span data-ttu-id="a0227-140">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="a0227-140">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="a0227-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0227-141">Response</span></span>

<span data-ttu-id="a0227-142">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект openShift](../resources/openshift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0227-142">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0227-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0227-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0227-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0227-144">Request</span></span>

<span data-ttu-id="a0227-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0227-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0227-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0227-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
Content-type: application/json

{
"schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
"sharedOpenShift": {
"notes": "Inventory Management",
"openSlotCount":5,
"displayName": "Field shift",
"startDateTime": "2018-10-04T00:58:45.340Z",
"endDateTime": "2018-10-04T09:50:45.332Z",
"theme": "white",
"activities": [
{
"isPaid": true,
"startDateTime": "2018-10-04T00:58:45.340Z",
"endDateTime": "2018-10-04T01:58:45.340Z",
"code": "",
"displayName": "Lunch"
}
]
},
"draftOpenShift": null
}
```
# <a name="c"></a>[<span data-ttu-id="a0227-147">C#</span><span class="sxs-lookup"><span data-stu-id="a0227-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0227-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0227-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0227-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0227-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0227-150">Java</span><span class="sxs-lookup"><span data-stu-id="a0227-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0227-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0227-151">Response</span></span>

<span data-ttu-id="a0227-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a0227-152">The following is an example of the response.</span></span>

> <span data-ttu-id="a0227-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0227-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "sharedOpenShift": {
  "notes": "Inventory Management",
  "openSlotCount":5,
  "displayName": "Day shift",
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T09:50:45.332Z",
  "theme": "white",
  "activities": [
  {
  "isPaid": true,
  "startDateTime": "2018-10-04T00:58:45.340Z",
  "endDateTime": "2018-10-04T01:58:45.340Z",
  "code": "",
  "displayName": "Lunch"
  }
  ]
  },
  "draftOpenShift": null,
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
  "application": null,
  "device": null,
  "conversation": null,
  "user": {
  "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
  "displayName": "John Doe"
  }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update openshift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


