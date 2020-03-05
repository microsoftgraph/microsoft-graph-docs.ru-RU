---
title: Удаление Опеншифт
description: Удаление объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0489ff3ee4c79a385ee0c5e14f8e81698adbf7ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456427"
---
# <a name="delete-openshift"></a><span data-ttu-id="c88d7-103">Удаление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="c88d7-103">Delete openShift</span></span>

<span data-ttu-id="c88d7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c88d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88d7-105">Удаление объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="c88d7-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c88d7-106">Permissions</span></span>

<span data-ttu-id="c88d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c88d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c88d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c88d7-109">Permission type</span></span>                        | <span data-ttu-id="c88d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c88d7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c88d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c88d7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c88d7-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c88d7-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c88d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c88d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c88d7-114">Not supported.</span></span> |
| <span data-ttu-id="c88d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c88d7-115">Application</span></span>                            | <span data-ttu-id="c88d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c88d7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c88d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="c88d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c88d7-118">Request headers</span></span>

| <span data-ttu-id="c88d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c88d7-119">Name</span></span>          | <span data-ttu-id="c88d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c88d7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c88d7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c88d7-121">Authorization</span></span> | <span data-ttu-id="c88d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c88d7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c88d7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c88d7-124">Request body</span></span>

<span data-ttu-id="c88d7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c88d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88d7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c88d7-126">Response</span></span>

<span data-ttu-id="c88d7-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c88d7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c88d7-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c88d7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c88d7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c88d7-130">Request</span></span>

<span data-ttu-id="c88d7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c88d7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c88d7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c88d7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
```
# <a name="c"></a>[<span data-ttu-id="c88d7-133">C#</span><span class="sxs-lookup"><span data-stu-id="c88d7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c88d7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c88d7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c88d7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c88d7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c88d7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c88d7-136">Response</span></span>

<span data-ttu-id="c88d7-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c88d7-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
