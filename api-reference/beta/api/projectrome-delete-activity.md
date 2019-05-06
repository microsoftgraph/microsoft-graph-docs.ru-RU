---
title: Удаление действия
description: Удаление существующего действия пользователя для вашего приложения.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: ba1c87c229fe76f20c85c164b7d788f7df9316b8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33610828"
---
# <a name="delete-an-activity"></a><span data-ttu-id="bae49-103">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="bae49-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bae49-104">Удаление существующего действия пользователя для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="bae49-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="bae49-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bae49-105">Permissions</span></span>

<span data-ttu-id="bae49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bae49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bae49-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bae49-108">Permission type</span></span>      | <span data-ttu-id="bae49-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bae49-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bae49-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bae49-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bae49-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bae49-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="bae49-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bae49-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bae49-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="bae49-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="bae49-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bae49-114">Application</span></span> | <span data-ttu-id="bae49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bae49-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bae49-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bae49-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bae49-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bae49-117">Request headers</span></span>

|<span data-ttu-id="bae49-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bae49-118">Name</span></span> | <span data-ttu-id="bae49-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bae49-119">Type</span></span> | <span data-ttu-id="bae49-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bae49-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bae49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae49-121">Authorization</span></span> | <span data-ttu-id="bae49-122">string</span><span class="sxs-lookup"><span data-stu-id="bae49-122">string</span></span> | <span data-ttu-id="bae49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bae49-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae49-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bae49-125">Request body</span></span>

<span data-ttu-id="bae49-126">Текст запроса отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bae49-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="bae49-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bae49-127">Response</span></span>

<span data-ttu-id="bae49-128">В случае успешного выполнения этот метод возвращает `204 No Content` код отклика, если действие было удалено.</span><span class="sxs-lookup"><span data-stu-id="bae49-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="bae49-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bae49-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bae49-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bae49-130">Request</span></span>

<span data-ttu-id="bae49-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bae49-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="bae49-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bae49-132">Response</span></span>

<span data-ttu-id="bae49-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bae49-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bae49-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bae49-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bae49-135">Языках</span><span class="sxs-lookup"><span data-stu-id="bae49-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_activity-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bae49-136">Язык</span><span class="sxs-lookup"><span data-stu-id="bae49-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_activity-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
