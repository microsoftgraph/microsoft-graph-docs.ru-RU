---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 641b7ea0f9ff3a1e705c565f60d9ed6ac88f4485
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455443"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="fc53f-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="fc53f-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc53f-104">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc53f-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc53f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc53f-105">Permissions</span></span>

<span data-ttu-id="fc53f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc53f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc53f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc53f-108">Permission type</span></span>      | <span data-ttu-id="fc53f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc53f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc53f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc53f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc53f-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fc53f-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fc53f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc53f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc53f-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="fc53f-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="fc53f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc53f-114">Application</span></span> | <span data-ttu-id="fc53f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc53f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc53f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc53f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fc53f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc53f-117">Request headers</span></span>

|<span data-ttu-id="fc53f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fc53f-118">Name</span></span> | <span data-ttu-id="fc53f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fc53f-119">Type</span></span> | <span data-ttu-id="fc53f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc53f-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fc53f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc53f-121">Authorization</span></span> | <span data-ttu-id="fc53f-122">string</span><span class="sxs-lookup"><span data-stu-id="fc53f-122">string</span></span> | <span data-ttu-id="fc53f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc53f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc53f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc53f-125">Request body</span></span>

<span data-ttu-id="fc53f-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="fc53f-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="fc53f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc53f-127">Response</span></span>

<span data-ttu-id="fc53f-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если элемент History был удален.</span><span class="sxs-lookup"><span data-stu-id="fc53f-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="fc53f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fc53f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc53f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc53f-130">Request</span></span>

<span data-ttu-id="fc53f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc53f-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc53f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc53f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc53f-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc53f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc53f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc53f-134">Response</span></span>

<span data-ttu-id="fc53f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc53f-135">Here is an example of the response.</span></span>

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
