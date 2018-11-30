---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
ms.openlocfilehash: 231a5dd1ffdeb09dab2ad08346b0202a1fe3d8fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026919"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="7ed08-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="7ed08-103">Delete a historyItem</span></span>

<span data-ttu-id="7ed08-104">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ed08-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ed08-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed08-105">Permissions</span></span>

<span data-ttu-id="7ed08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ed08-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed08-108">Permission type</span></span>      | <span data-ttu-id="7ed08-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ed08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ed08-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ed08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ed08-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7ed08-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7ed08-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ed08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ed08-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7ed08-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7ed08-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ed08-114">Application</span></span> | <span data-ttu-id="7ed08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed08-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ed08-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ed08-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ed08-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ed08-117">Request headers</span></span>

|<span data-ttu-id="7ed08-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7ed08-118">Name</span></span> | <span data-ttu-id="7ed08-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7ed08-119">Type</span></span> | <span data-ttu-id="7ed08-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed08-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7ed08-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ed08-121">Authorization</span></span> | <span data-ttu-id="7ed08-122">string</span><span class="sxs-lookup"><span data-stu-id="7ed08-122">string</span></span> | <span data-ttu-id="7ed08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ed08-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed08-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ed08-125">Request body</span></span>

<span data-ttu-id="7ed08-126">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="7ed08-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="7ed08-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ed08-127">Response</span></span>

<span data-ttu-id="7ed08-128">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если журнал элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="7ed08-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="7ed08-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7ed08-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7ed08-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ed08-130">Request</span></span>

<span data-ttu-id="7ed08-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ed08-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="7ed08-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ed08-132">Response</span></span>

<span data-ttu-id="7ed08-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ed08-133">Here is an example of the response.</span></span>

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
  "tocPath": ""
}-->