---
title: Удаление historyItem
description: Удаление существующего элемента журнала для существующего действия пользователя.
localization_priority: Normal
ms.openlocfilehash: d9468034f3a98e949eeb9f2da28c4a74c42cd991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834981"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="d0da5-103">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="d0da5-103">Delete a historyItem</span></span>

> <span data-ttu-id="d0da5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0da5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0da5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0da5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0da5-106">Удаление существующего элемента журнала для существующего действия пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0da5-106">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0da5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0da5-107">Permissions</span></span>

<span data-ttu-id="d0da5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0da5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d0da5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0da5-110">Permission type</span></span>      | <span data-ttu-id="d0da5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0da5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0da5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0da5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0da5-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d0da5-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d0da5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0da5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0da5-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d0da5-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d0da5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0da5-116">Application</span></span> | <span data-ttu-id="d0da5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0da5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0da5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0da5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d0da5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0da5-119">Request headers</span></span>

|<span data-ttu-id="d0da5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d0da5-120">Name</span></span> | <span data-ttu-id="d0da5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d0da5-121">Type</span></span> | <span data-ttu-id="d0da5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d0da5-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d0da5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0da5-123">Authorization</span></span> | <span data-ttu-id="d0da5-124">string</span><span class="sxs-lookup"><span data-stu-id="d0da5-124">string</span></span> | <span data-ttu-id="d0da5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0da5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0da5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0da5-127">Request body</span></span>

<span data-ttu-id="d0da5-128">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="d0da5-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="d0da5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0da5-129">Response</span></span>

<span data-ttu-id="d0da5-130">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если журнал элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="d0da5-130">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="d0da5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d0da5-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d0da5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0da5-132">Request</span></span>

<span data-ttu-id="d0da5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0da5-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="d0da5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0da5-134">Response</span></span>

<span data-ttu-id="d0da5-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0da5-135">Here is an example of the response.</span></span>

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
