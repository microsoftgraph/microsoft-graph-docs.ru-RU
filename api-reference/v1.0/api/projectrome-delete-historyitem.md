---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 5fc0088b5e8d814e15cb6231956bd8deff266b41
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458609"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="420ff-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="420ff-103">Delete a historyItem</span></span>

<span data-ttu-id="420ff-104">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="420ff-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="420ff-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="420ff-105">Permissions</span></span>

<span data-ttu-id="420ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="420ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="420ff-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="420ff-108">Permission type</span></span>      | <span data-ttu-id="420ff-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="420ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="420ff-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="420ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="420ff-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="420ff-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="420ff-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="420ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="420ff-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="420ff-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="420ff-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="420ff-114">Application</span></span> | <span data-ttu-id="420ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="420ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="420ff-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="420ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="420ff-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="420ff-117">Request headers</span></span>

|<span data-ttu-id="420ff-118">Имя</span><span class="sxs-lookup"><span data-stu-id="420ff-118">Name</span></span> | <span data-ttu-id="420ff-119">Тип</span><span class="sxs-lookup"><span data-stu-id="420ff-119">Type</span></span> | <span data-ttu-id="420ff-120">Описание</span><span class="sxs-lookup"><span data-stu-id="420ff-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="420ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="420ff-121">Authorization</span></span> | <span data-ttu-id="420ff-122">string</span><span class="sxs-lookup"><span data-stu-id="420ff-122">string</span></span> | <span data-ttu-id="420ff-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="420ff-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="420ff-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="420ff-125">Request body</span></span>

<span data-ttu-id="420ff-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="420ff-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="420ff-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="420ff-127">Response</span></span>

<span data-ttu-id="420ff-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если элемент History был удален.</span><span class="sxs-lookup"><span data-stu-id="420ff-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="420ff-129">Пример</span><span class="sxs-lookup"><span data-stu-id="420ff-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="420ff-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="420ff-130">Request</span></span>

<span data-ttu-id="420ff-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="420ff-131">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="420ff-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="420ff-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="420ff-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="420ff-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-historyitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="420ff-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="420ff-134">Response</span></span>

<span data-ttu-id="420ff-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="420ff-135">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
