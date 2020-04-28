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
# <a name="delete-openshift"></a><span data-ttu-id="c4dd8-103">Удаление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="c4dd8-103">Delete openShift</span></span>

<span data-ttu-id="c4dd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4dd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4dd8-105">Удаление объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="c4dd8-105">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4dd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4dd8-106">Permissions</span></span>

<span data-ttu-id="c4dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4dd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4dd8-109">Permission type</span></span>                        | <span data-ttu-id="c4dd8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4dd8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c4dd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4dd8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4dd8-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4dd8-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c4dd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4dd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4dd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-114">Not supported.</span></span> |
| <span data-ttu-id="c4dd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4dd8-115">Application</span></span>                            | <span data-ttu-id="c4dd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4dd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4dd8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="c4dd8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4dd8-118">Request headers</span></span>

| <span data-ttu-id="c4dd8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4dd8-119">Name</span></span>          | <span data-ttu-id="c4dd8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4dd8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c4dd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4dd8-121">Authorization</span></span> | <span data-ttu-id="c4dd8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4dd8-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4dd8-124">Request body</span></span>

<span data-ttu-id="c4dd8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4dd8-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4dd8-126">Response</span></span>

<span data-ttu-id="c4dd8-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4dd8-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4dd8-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4dd8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4dd8-130">Request</span></span>

<span data-ttu-id="c4dd8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4dd8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4dd8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
```
# <a name="c"></a>[<span data-ttu-id="c4dd8-133">C#</span><span class="sxs-lookup"><span data-stu-id="c4dd8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4dd8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4dd8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4dd8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4dd8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c4dd8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4dd8-136">Response</span></span>

<span data-ttu-id="c4dd8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4dd8-137">The following is an example of the response.</span></span>

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
