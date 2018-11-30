---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
ms.openlocfilehash: a4b32e00719772f6dcfb715fa69350edf9a8b48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025296"
---
# <a name="delete-an-activity"></a><span data-ttu-id="903aa-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="903aa-103">Delete an activity</span></span>

<span data-ttu-id="903aa-104">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="903aa-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="903aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="903aa-105">Permissions</span></span>

<span data-ttu-id="903aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="903aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="903aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="903aa-108">Permission type</span></span>      | <span data-ttu-id="903aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="903aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="903aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="903aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="903aa-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="903aa-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="903aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="903aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="903aa-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="903aa-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="903aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="903aa-114">Application</span></span> | <span data-ttu-id="903aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="903aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="903aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="903aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="903aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="903aa-117">Request headers</span></span>

|<span data-ttu-id="903aa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="903aa-118">Name</span></span> | <span data-ttu-id="903aa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="903aa-119">Type</span></span> | <span data-ttu-id="903aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="903aa-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="903aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="903aa-121">Authorization</span></span> | <span data-ttu-id="903aa-122">string</span><span class="sxs-lookup"><span data-stu-id="903aa-122">string</span></span> | <span data-ttu-id="903aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="903aa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="903aa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="903aa-125">Request body</span></span>

<span data-ttu-id="903aa-126">Нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="903aa-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="903aa-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="903aa-127">Response</span></span>

<span data-ttu-id="903aa-128">Успешно завершена, этот метод возвращает `204 No Content` код ответа, если действие был удален.</span><span class="sxs-lookup"><span data-stu-id="903aa-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="903aa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="903aa-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="903aa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="903aa-130">Request</span></span>

<span data-ttu-id="903aa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="903aa-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="903aa-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="903aa-132">Response</span></span>

<span data-ttu-id="903aa-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="903aa-133">Here is an example of the response.</span></span>

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