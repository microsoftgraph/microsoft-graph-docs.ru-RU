---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 8b4bf0b09cb5796e1db8e22ced7e471bdd5117f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925751"
---
# <a name="delete-an-activity"></a><span data-ttu-id="7b286-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="7b286-103">Delete an activity</span></span>

> <span data-ttu-id="7b286-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b286-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b286-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b286-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b286-106">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="7b286-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b286-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b286-107">Permissions</span></span>

<span data-ttu-id="7b286-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b286-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7b286-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b286-110">Permission type</span></span>      | <span data-ttu-id="7b286-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b286-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b286-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b286-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b286-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7b286-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7b286-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b286-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b286-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="7b286-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="7b286-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b286-116">Application</span></span> | <span data-ttu-id="7b286-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b286-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b286-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b286-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7b286-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b286-119">Request headers</span></span>

|<span data-ttu-id="7b286-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7b286-120">Name</span></span> | <span data-ttu-id="7b286-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7b286-121">Type</span></span> | <span data-ttu-id="7b286-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7b286-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7b286-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b286-123">Authorization</span></span> | <span data-ttu-id="7b286-124">строка</span><span class="sxs-lookup"><span data-stu-id="7b286-124">string</span></span> | <span data-ttu-id="7b286-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b286-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b286-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b286-127">Request body</span></span>

<span data-ttu-id="7b286-128">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="7b286-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="7b286-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b286-129">Response</span></span>

<span data-ttu-id="7b286-130">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если действие был удален.</span><span class="sxs-lookup"><span data-stu-id="7b286-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="7b286-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7b286-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7b286-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b286-132">Request</span></span>

<span data-ttu-id="7b286-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b286-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="7b286-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b286-134">Response</span></span>

<span data-ttu-id="7b286-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b286-135">Here is an example of the response.</span></span>

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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
