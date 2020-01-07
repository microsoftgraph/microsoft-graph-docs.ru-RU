---
title: Удаление Опеншифт
description: Удаление объекта Опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fcd91c57079641097abfbf9674ca204c3909714e
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951925"
---
# <a name="delete-openshift"></a><span data-ttu-id="b4a76-103">Удаление Опеншифт</span><span class="sxs-lookup"><span data-stu-id="b4a76-103">Delete openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4a76-104">Удаление объекта [опеншифт](../resources/openshift.md) .</span><span class="sxs-lookup"><span data-stu-id="b4a76-104">Delete an [openShift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4a76-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a76-105">Permissions</span></span>

<span data-ttu-id="b4a76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4a76-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a76-108">Permission type</span></span>                        | <span data-ttu-id="b4a76-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a76-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b4a76-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a76-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4a76-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a76-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b4a76-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4a76-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a76-113">Not supported.</span></span> |
| <span data-ttu-id="b4a76-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4a76-114">Application</span></span>                            | <span data-ttu-id="b4a76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a76-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4a76-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a76-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/openShifts/{openShiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b4a76-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4a76-117">Request headers</span></span>

| <span data-ttu-id="b4a76-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b4a76-118">Name</span></span>          | <span data-ttu-id="b4a76-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a76-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b4a76-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4a76-120">Authorization</span></span> | <span data-ttu-id="b4a76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a76-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4a76-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4a76-123">Request body</span></span>

<span data-ttu-id="b4a76-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4a76-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4a76-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a76-125">Response</span></span>

<span data-ttu-id="b4a76-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4a76-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4a76-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4a76-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4a76-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a76-129">Request</span></span>

<span data-ttu-id="b4a76-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a76-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4a76-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4a76-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_openshift"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts/{openShiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4a76-132">C#</span><span class="sxs-lookup"><span data-stu-id="b4a76-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-openshift-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4a76-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4a76-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-openshift-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4a76-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4a76-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-openshift-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4a76-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a76-135">Response</span></span>

<span data-ttu-id="b4a76-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4a76-136">The following is an example of the response.</span></span>

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
