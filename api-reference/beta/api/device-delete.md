---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6f225cc410515b40952e64fb13d053b2eeb25fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417699"
---
# <a name="delete-device"></a><span data-ttu-id="c3972-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="c3972-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3972-104">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="c3972-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3972-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3972-105">Permissions</span></span>
<span data-ttu-id="c3972-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3972-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3972-108">Permission type</span></span>      | <span data-ttu-id="c3972-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3972-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3972-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3972-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3972-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3972-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c3972-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3972-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3972-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3972-113">Not supported.</span></span>    |
|<span data-ttu-id="c3972-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3972-114">Application</span></span> | <span data-ttu-id="c3972-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3972-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3972-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3972-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="c3972-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="c3972-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3972-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3972-118">Request headers</span></span>
| <span data-ttu-id="c3972-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c3972-119">Name</span></span>       | <span data-ttu-id="c3972-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c3972-120">Type</span></span> | <span data-ttu-id="c3972-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3972-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3972-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3972-122">Authorization</span></span>  | <span data-ttu-id="c3972-123">string</span><span class="sxs-lookup"><span data-stu-id="c3972-123">string</span></span>  | <span data-ttu-id="c3972-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3972-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3972-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3972-126">Request body</span></span>
<span data-ttu-id="c3972-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3972-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3972-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3972-128">Response</span></span>

<span data-ttu-id="c3972-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c3972-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3972-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3972-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3972-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3972-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3972-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3972-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3972-134">C#</span><span class="sxs-lookup"><span data-stu-id="c3972-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3972-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3972-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3972-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c3972-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3972-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3972-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
