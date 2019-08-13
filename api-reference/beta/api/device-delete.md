---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a1557710de6bd74735e646f5c28f88bd6940702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319666"
---
# <a name="delete-device"></a><span data-ttu-id="b73bf-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="b73bf-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b73bf-104">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="b73bf-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="b73bf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b73bf-105">Permissions</span></span>
<span data-ttu-id="b73bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b73bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b73bf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b73bf-108">Permission type</span></span>      | <span data-ttu-id="b73bf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b73bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b73bf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b73bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b73bf-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b73bf-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b73bf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b73bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b73bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b73bf-113">Not supported.</span></span>    |
|<span data-ttu-id="b73bf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b73bf-114">Application</span></span> | <span data-ttu-id="b73bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b73bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b73bf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b73bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="b73bf-117">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="b73bf-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b73bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b73bf-118">Request headers</span></span>
| <span data-ttu-id="b73bf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b73bf-119">Name</span></span>       | <span data-ttu-id="b73bf-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b73bf-120">Type</span></span> | <span data-ttu-id="b73bf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b73bf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b73bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b73bf-122">Authorization</span></span>  | <span data-ttu-id="b73bf-123">string</span><span class="sxs-lookup"><span data-stu-id="b73bf-123">string</span></span>  | <span data-ttu-id="b73bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b73bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b73bf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b73bf-126">Request body</span></span>
<span data-ttu-id="b73bf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b73bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b73bf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b73bf-128">Response</span></span>

<span data-ttu-id="b73bf-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b73bf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b73bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b73bf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b73bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b73bf-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b73bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b73bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b73bf-134">C#</span><span class="sxs-lookup"><span data-stu-id="b73bf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b73bf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b73bf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b73bf-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b73bf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b73bf-137">Java</span><span class="sxs-lookup"><span data-stu-id="b73bf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b73bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b73bf-138">Response</span></span>

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
