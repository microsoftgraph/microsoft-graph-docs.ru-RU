---
title: Обновление Опеншифт
description: Обновление свойств объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fd1b265a1f4d4169dfb16ec8265ae2152cfd5b83
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/04/2020
ms.locfileid: "44345774"
---
# <a name="update-openshift"></a><span data-ttu-id="96d41-103">Обновление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="96d41-103">Update openShift</span></span>

<span data-ttu-id="96d41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96d41-105">Обновление свойств объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="96d41-105">Update the properties of an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96d41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96d41-106">Permissions</span></span>

<span data-ttu-id="96d41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96d41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d41-109">Permission type</span></span>                        | <span data-ttu-id="96d41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d41-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96d41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d41-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96d41-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="96d41-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="96d41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96d41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d41-114">Not supported.</span></span> |
| <span data-ttu-id="96d41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96d41-115">Application</span></span>                            | <span data-ttu-id="96d41-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d41-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="96d41-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="96d41-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="96d41-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="96d41-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="96d41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d41-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="96d41-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96d41-120">Request headers</span></span>

| <span data-ttu-id="96d41-121">Имя</span><span class="sxs-lookup"><span data-stu-id="96d41-121">Name</span></span>       | <span data-ttu-id="96d41-122">Описание</span><span class="sxs-lookup"><span data-stu-id="96d41-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="96d41-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96d41-123">Authorization</span></span> | <span data-ttu-id="96d41-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96d41-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96d41-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96d41-126">Content-type</span></span> | <span data-ttu-id="96d41-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96d41-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96d41-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96d41-129">Request body</span></span>

<span data-ttu-id="96d41-130">Предоставьте измененный объект [опеншифт](../resources/openshift.md) в тексте запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96d41-130">Provide the modified [openShift](../resources/openshift.md) object in the request body for this method.</span></span>

| <span data-ttu-id="96d41-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="96d41-131">Property</span></span>     | <span data-ttu-id="96d41-132">Тип</span><span class="sxs-lookup"><span data-stu-id="96d41-132">Type</span></span>        | <span data-ttu-id="96d41-133">Описание</span><span class="sxs-lookup"><span data-stu-id="96d41-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96d41-134">драфтопеншифт</span><span class="sxs-lookup"><span data-stu-id="96d41-134">draftOpenShift</span></span>|<span data-ttu-id="96d41-135">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="96d41-135">openShiftItem</span></span>|<span data-ttu-id="96d41-136">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="96d41-136">An unpublished open shift.</span></span>|
|<span data-ttu-id="96d41-137">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="96d41-137">schedulingGroupId</span></span>|<span data-ttu-id="96d41-138">String</span><span class="sxs-lookup"><span data-stu-id="96d41-138">String</span></span>| <span data-ttu-id="96d41-139">Планирование кода группы.</span><span class="sxs-lookup"><span data-stu-id="96d41-139">Scheduling group ID.</span></span> |
|<span data-ttu-id="96d41-140">шаредопеншифт</span><span class="sxs-lookup"><span data-stu-id="96d41-140">sharedOpenShift</span></span>|<span data-ttu-id="96d41-141">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="96d41-141">openShiftItem</span></span>|<span data-ttu-id="96d41-142">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="96d41-142">A published open shift.</span></span>|

## <a name="response"></a><span data-ttu-id="96d41-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d41-143">Response</span></span>

<span data-ttu-id="96d41-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [опеншифт](../resources/openshift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96d41-144">If successful, this method returns a `200 OK` response code and an updated [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96d41-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="96d41-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96d41-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d41-146">Request</span></span>

<span data-ttu-id="96d41-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d41-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96d41-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="96d41-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="96d41-149">C#</span><span class="sxs-lookup"><span data-stu-id="96d41-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96d41-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96d41-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96d41-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96d41-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96d41-152">Java</span><span class="sxs-lookup"><span data-stu-id="96d41-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="96d41-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="96d41-153">Response</span></span>

<span data-ttu-id="96d41-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96d41-154">The following is an example of the response.</span></span>

> <span data-ttu-id="96d41-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96d41-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
