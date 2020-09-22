---
title: Удаление Опеншифт
description: Удаление объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b64df2cc2af979f783688bb8d83fa6e17fc1b834
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057145"
---
# <a name="delete-openshift"></a><span data-ttu-id="277e8-103">Удаление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="277e8-103">Delete openShift</span></span>

<span data-ttu-id="277e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="277e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="277e8-105">Удаление объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="277e8-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="277e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="277e8-106">Permissions</span></span>

<span data-ttu-id="277e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="277e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="277e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="277e8-109">Permission type</span></span>                        | <span data-ttu-id="277e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="277e8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="277e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="277e8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="277e8-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="277e8-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="277e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="277e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="277e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="277e8-114">Not supported.</span></span> |
| <span data-ttu-id="277e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="277e8-115">Application</span></span>                            | <span data-ttu-id="277e8-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="277e8-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="277e8-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="277e8-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="277e8-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="277e8-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="277e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="277e8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="277e8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="277e8-120">Request headers</span></span>

| <span data-ttu-id="277e8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="277e8-121">Name</span></span>          | <span data-ttu-id="277e8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="277e8-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="277e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="277e8-123">Authorization</span></span> | <span data-ttu-id="277e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="277e8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="277e8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="277e8-126">Request body</span></span>

<span data-ttu-id="277e8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="277e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="277e8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="277e8-128">Response</span></span>

<span data-ttu-id="277e8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="277e8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="277e8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="277e8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="277e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="277e8-132">Request</span></span>

<span data-ttu-id="277e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="277e8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="277e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="277e8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8
```
# <a name="c"></a>[<span data-ttu-id="277e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="277e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="277e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="277e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="277e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="277e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="277e8-138">Java</span><span class="sxs-lookup"><span data-stu-id="277e8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-openshift-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="277e8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="277e8-139">Response</span></span>

<span data-ttu-id="277e8-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="277e8-140">The following is an example of the response.</span></span>

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
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

