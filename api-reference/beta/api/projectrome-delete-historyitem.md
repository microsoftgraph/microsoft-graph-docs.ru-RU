---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ''
ms.openlocfilehash: 852d4f7c13dd6bf710d2ec429e0a1313ff33e46f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454902"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="5af9b-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="5af9b-103">Delete a historyItem</span></span>

<span data-ttu-id="5af9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5af9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5af9b-105">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="5af9b-105">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="5af9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5af9b-106">Permissions</span></span>

<span data-ttu-id="5af9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5af9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5af9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5af9b-109">Permission type</span></span>      | <span data-ttu-id="5af9b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5af9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5af9b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5af9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5af9b-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5af9b-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5af9b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5af9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5af9b-114">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5af9b-114">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5af9b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5af9b-115">Application</span></span> | <span data-ttu-id="5af9b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5af9b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5af9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5af9b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5af9b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5af9b-118">Request headers</span></span>

|<span data-ttu-id="5af9b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5af9b-119">Name</span></span> | <span data-ttu-id="5af9b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5af9b-120">Type</span></span> | <span data-ttu-id="5af9b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5af9b-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5af9b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5af9b-122">Authorization</span></span> | <span data-ttu-id="5af9b-123">string</span><span class="sxs-lookup"><span data-stu-id="5af9b-123">string</span></span> | <span data-ttu-id="5af9b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5af9b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af9b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5af9b-126">Request body</span></span>

<span data-ttu-id="5af9b-127">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5af9b-127">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="5af9b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5af9b-128">Response</span></span>

<span data-ttu-id="5af9b-129">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если элемент History был удален.</span><span class="sxs-lookup"><span data-stu-id="5af9b-129">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="5af9b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5af9b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5af9b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5af9b-131">Request</span></span>

<span data-ttu-id="5af9b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5af9b-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5af9b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5af9b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```
# <a name="objective-c"></a>[<span data-ttu-id="5af9b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5af9b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5af9b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5af9b-135">Response</span></span>

<span data-ttu-id="5af9b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5af9b-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
