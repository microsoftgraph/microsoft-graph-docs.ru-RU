---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: cbe12a373f06c2893a5ca202247865f4ce4a8f52
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574203"
---
# <a name="delete-an-activity"></a><span data-ttu-id="bc41c-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="bc41c-103">Delete an activity</span></span>

<span data-ttu-id="bc41c-104">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="bc41c-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc41c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc41c-105">Permissions</span></span>

<span data-ttu-id="bc41c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bc41c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc41c-108">Permission type</span></span>      | <span data-ttu-id="bc41c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc41c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc41c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc41c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc41c-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bc41c-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="bc41c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc41c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc41c-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bc41c-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="bc41c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc41c-114">Application</span></span> | <span data-ttu-id="bc41c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc41c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc41c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc41c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bc41c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc41c-117">Request headers</span></span>

|<span data-ttu-id="bc41c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bc41c-118">Name</span></span> | <span data-ttu-id="bc41c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bc41c-119">Type</span></span> | <span data-ttu-id="bc41c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc41c-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bc41c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc41c-121">Authorization</span></span> | <span data-ttu-id="bc41c-122">string</span><span class="sxs-lookup"><span data-stu-id="bc41c-122">string</span></span> | <span data-ttu-id="bc41c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc41c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc41c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc41c-125">Request body</span></span>

<span data-ttu-id="bc41c-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bc41c-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="bc41c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc41c-127">Response</span></span>

<span data-ttu-id="bc41c-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="bc41c-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="bc41c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bc41c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc41c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc41c-130">Request</span></span>

<span data-ttu-id="bc41c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc41c-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="bc41c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc41c-132">Response</span></span>

<span data-ttu-id="bc41c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc41c-133">Here is an example of the response.</span></span>

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
