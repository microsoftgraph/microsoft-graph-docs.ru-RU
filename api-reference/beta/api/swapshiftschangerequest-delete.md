---
title: Удаление Свапшифтсчанжерекуест
description: Удаление объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 09e7a6eaa03525d20479731fc07d691e8f70f093
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870866"
---
# <a name="delete-swapshiftschangerequest"></a><span data-ttu-id="db47c-103">Удаление Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="db47c-103">Delete swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db47c-104">Удаление объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="db47c-104">Delete a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db47c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db47c-105">Permissions</span></span>

<span data-ttu-id="db47c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db47c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db47c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db47c-108">Permission type</span></span>                        | <span data-ttu-id="db47c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db47c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db47c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db47c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="db47c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db47c-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="db47c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db47c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db47c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db47c-113">Not supported.</span></span> |
|<span data-ttu-id="db47c-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="db47c-114">Application</span></span> | <span data-ttu-id="db47c-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="db47c-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="db47c-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="db47c-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="db47c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db47c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="db47c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db47c-118">Request headers</span></span>

| <span data-ttu-id="db47c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="db47c-119">Name</span></span>          | <span data-ttu-id="db47c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="db47c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db47c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db47c-121">Authorization</span></span> | <span data-ttu-id="db47c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db47c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db47c-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db47c-124">Request body</span></span>

<span data-ttu-id="db47c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db47c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db47c-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="db47c-126">Response</span></span>

<span data-ttu-id="db47c-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db47c-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db47c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="db47c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db47c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="db47c-130">Request</span></span>

<span data-ttu-id="db47c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db47c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db47c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="db47c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_swapshiftschangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db47c-133">C#</span><span class="sxs-lookup"><span data-stu-id="db47c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-swapshiftschangerequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db47c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db47c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-swapshiftschangerequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db47c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db47c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-swapshiftschangerequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db47c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db47c-136">Response</span></span>

<span data-ttu-id="db47c-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db47c-137">The following is an example of the response.</span></span>

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
  "description": "Delete swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
