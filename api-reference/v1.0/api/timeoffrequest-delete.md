---
title: Удаление Тимеоффрекуест
description: Удаление объекта Тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5af597174d6146c50d88a3038af1af0158c931
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044069"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="67bca-103">Удаление Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="67bca-103">Delete timeOffRequest</span></span>

<span data-ttu-id="67bca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67bca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67bca-105">Удаление объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="67bca-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67bca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67bca-106">Permissions</span></span>

<span data-ttu-id="67bca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="67bca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67bca-109">Permission type</span></span>                        | <span data-ttu-id="67bca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67bca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="67bca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67bca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67bca-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="67bca-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="67bca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67bca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67bca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67bca-114">Not supported.</span></span>    |
|<span data-ttu-id="67bca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67bca-115">Application</span></span> | <span data-ttu-id="67bca-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bca-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="67bca-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="67bca-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="67bca-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="67bca-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="67bca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67bca-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="67bca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67bca-120">Request headers</span></span>

| <span data-ttu-id="67bca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="67bca-121">Name</span></span>          | <span data-ttu-id="67bca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="67bca-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="67bca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67bca-123">Authorization</span></span> | <span data-ttu-id="67bca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67bca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67bca-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67bca-126">Request body</span></span>

<span data-ttu-id="67bca-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67bca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67bca-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="67bca-128">Response</span></span>

<span data-ttu-id="67bca-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="67bca-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67bca-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="67bca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67bca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="67bca-132">Request</span></span>

<span data-ttu-id="67bca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67bca-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67bca-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="67bca-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="67bca-135">C#</span><span class="sxs-lookup"><span data-stu-id="67bca-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67bca-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67bca-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67bca-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67bca-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67bca-138">Java</span><span class="sxs-lookup"><span data-stu-id="67bca-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="67bca-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="67bca-139">Response</span></span>

<span data-ttu-id="67bca-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="67bca-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

