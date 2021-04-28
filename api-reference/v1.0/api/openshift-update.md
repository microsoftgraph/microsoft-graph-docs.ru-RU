---
title: Обновление openShift
description: Обновление свойств объекта openShift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16d25b1c0056134ad0517630a8fd65547944f300
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051321"
---
# <a name="update-openshift"></a><span data-ttu-id="a782f-103">Обновление openShift</span><span class="sxs-lookup"><span data-stu-id="a782f-103">Update openShift</span></span>

<span data-ttu-id="a782f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a782f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a782f-105">Обновление свойств объекта [openShift.](../resources/openshift.md)</span><span class="sxs-lookup"><span data-stu-id="a782f-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a782f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a782f-106">Permissions</span></span>

<span data-ttu-id="a782f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a782f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a782f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a782f-109">Permission type</span></span>                        | <span data-ttu-id="a782f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a782f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a782f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a782f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a782f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a782f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a782f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a782f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a782f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a782f-114">Not supported.</span></span> |
| <span data-ttu-id="a782f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a782f-115">Application</span></span>                            | <span data-ttu-id="a782f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a782f-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="a782f-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a782f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a782f-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="a782f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a782f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a782f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="a782f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a782f-120">Request headers</span></span>

| <span data-ttu-id="a782f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a782f-121">Name</span></span>       | <span data-ttu-id="a782f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a782f-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a782f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a782f-123">Authorization</span></span> | <span data-ttu-id="a782f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a782f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a782f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a782f-126">Content-type</span></span> | <span data-ttu-id="a782f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a782f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a782f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a782f-129">Request body</span></span>

<span data-ttu-id="a782f-130">Предокажи измененный [объект openShift](../resources/openshift.md) в теле запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a782f-130">Provide the modified [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="a782f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a782f-131">Property</span></span>     | <span data-ttu-id="a782f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a782f-132">Type</span></span>        | <span data-ttu-id="a782f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a782f-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a782f-134">draftOpenShift</span><span class="sxs-lookup"><span data-stu-id="a782f-134">draftOpenShift</span></span>|<span data-ttu-id="a782f-135">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a782f-135">openShiftItem</span></span>|<span data-ttu-id="a782f-136">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="a782f-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="a782f-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="a782f-137">schedulingGroupId</span></span>|<span data-ttu-id="a782f-138">String</span><span class="sxs-lookup"><span data-stu-id="a782f-138">String</span></span>| <span data-ttu-id="a782f-139">Планирование группового ИД.</span><span class="sxs-lookup"><span data-stu-id="a782f-139">Scheduling group ID.</span></span> |
|<span data-ttu-id="a782f-140">sharedOpenShift</span><span class="sxs-lookup"><span data-stu-id="a782f-140">sharedOpenShift</span></span>|<span data-ttu-id="a782f-141">openShiftItem</span><span class="sxs-lookup"><span data-stu-id="a782f-141">openShiftItem</span></span>|<span data-ttu-id="a782f-142">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="a782f-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="a782f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a782f-143">Response</span></span>

<span data-ttu-id="a782f-144">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект openShift](../resources/openshift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a782f-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a782f-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="a782f-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a782f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a782f-146">Request</span></span>

<span data-ttu-id="a782f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a782f-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a782f-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a782f-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_openshift"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
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
# <a name="c"></a>[<span data-ttu-id="a782f-149">C#</span><span class="sxs-lookup"><span data-stu-id="a782f-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a782f-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a782f-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a782f-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a782f-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a782f-152">Java</span><span class="sxs-lookup"><span data-stu-id="a782f-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="a782f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a782f-153">Response</span></span>

<span data-ttu-id="a782f-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a782f-154">The following is an example of the response.</span></span>

> <span data-ttu-id="a782f-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a782f-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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

