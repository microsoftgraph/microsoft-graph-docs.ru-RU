---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.openlocfilehash: 92b927dbb568221003fdaff108640cf24520d182
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819553"
---
# <a name="delete-an-activity"></a><span data-ttu-id="022f3-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="022f3-103">Delete an activity</span></span>

> <span data-ttu-id="022f3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="022f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="022f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="022f3-106">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="022f3-106">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="022f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="022f3-107">Permissions</span></span>

<span data-ttu-id="022f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="022f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="022f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="022f3-110">Permission type</span></span>      | <span data-ttu-id="022f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="022f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="022f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="022f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="022f3-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="022f3-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="022f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="022f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="022f3-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="022f3-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="022f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="022f3-116">Application</span></span> | <span data-ttu-id="022f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="022f3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="022f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="022f3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="022f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="022f3-119">Request headers</span></span>

|<span data-ttu-id="022f3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="022f3-120">Name</span></span> | <span data-ttu-id="022f3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="022f3-121">Type</span></span> | <span data-ttu-id="022f3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="022f3-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="022f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="022f3-123">Authorization</span></span> | <span data-ttu-id="022f3-124">string</span><span class="sxs-lookup"><span data-stu-id="022f3-124">string</span></span> | <span data-ttu-id="022f3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="022f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="022f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="022f3-127">Request body</span></span>

<span data-ttu-id="022f3-128">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="022f3-128">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="022f3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="022f3-129">Response</span></span>

<span data-ttu-id="022f3-130">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если действие был удален.</span><span class="sxs-lookup"><span data-stu-id="022f3-130">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="022f3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="022f3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="022f3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="022f3-132">Request</span></span>

<span data-ttu-id="022f3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="022f3-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="022f3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="022f3-134">Response</span></span>

<span data-ttu-id="022f3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="022f3-135">Here is an example of the response.</span></span>

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
