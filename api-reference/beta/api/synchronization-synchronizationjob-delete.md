---
title: Удаление synchronizationJob
description: Остановить задание синхронизации и окончательно удалить все состояния, связанные с ним. Синхронизированные учетные записи остаются-является.
ms.openlocfilehash: d77101e8dfaf55a36dfd7260afb30aade81bbae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081233"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="6d39c-104">Удаление synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="6d39c-104">Delete synchronizationJob</span></span>

> <span data-ttu-id="6d39c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d39c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d39c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d39c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d39c-107">Остановить задание синхронизации и окончательно удалить все состояния, связанные с ним.</span><span class="sxs-lookup"><span data-stu-id="6d39c-107">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="6d39c-108">Синхронизированные учетные записи остаются-является.</span><span class="sxs-lookup"><span data-stu-id="6d39c-108">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d39c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d39c-109">Permissions</span></span>
<span data-ttu-id="6d39c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d39c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d39c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d39c-112">Permission type</span></span>                        | <span data-ttu-id="6d39c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d39c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d39c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d39c-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="6d39c-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d39c-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6d39c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d39c-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6d39c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d39c-117">Not supported.</span></span>  |
|<span data-ttu-id="6d39c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d39c-118">Application</span></span>                            |<span data-ttu-id="6d39c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d39c-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6d39c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d39c-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="6d39c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d39c-121">Request headers</span></span>

| <span data-ttu-id="6d39c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6d39c-122">Name</span></span>           | <span data-ttu-id="6d39c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6d39c-123">Type</span></span>    | <span data-ttu-id="6d39c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6d39c-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6d39c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d39c-125">Authorization</span></span>  | <span data-ttu-id="6d39c-126">string</span><span class="sxs-lookup"><span data-stu-id="6d39c-126">string</span></span>  | <span data-ttu-id="6d39c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d39c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d39c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d39c-129">Request body</span></span>

<span data-ttu-id="6d39c-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d39c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d39c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d39c-131">Response</span></span>

<span data-ttu-id="6d39c-132">В случае успеха возвращает `204 No Content` ответа.</span><span class="sxs-lookup"><span data-stu-id="6d39c-132">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="6d39c-133">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6d39c-133">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d39c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6d39c-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d39c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d39c-135">Request</span></span>
<span data-ttu-id="6d39c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d39c-136">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="6d39c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d39c-137">Response</span></span>
<span data-ttu-id="6d39c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d39c-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->