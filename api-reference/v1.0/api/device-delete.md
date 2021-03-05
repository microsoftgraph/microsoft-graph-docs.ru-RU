---
title: Удаление устройства
description: Удаление зарегистрированного устройства.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9aa477f6b5ef1505a6fe8b26a0afc980d0adc04e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434617"
---
# <a name="delete-device"></a><span data-ttu-id="b9300-103">Удаление устройства</span><span class="sxs-lookup"><span data-stu-id="b9300-103">Delete device</span></span>

<span data-ttu-id="b9300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9300-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9300-105">Удаление зарегистрированного устройства.</span><span class="sxs-lookup"><span data-stu-id="b9300-105">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9300-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9300-106">Permissions</span></span>
<span data-ttu-id="b9300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9300-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9300-109">Permission type</span></span>      | <span data-ttu-id="b9300-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9300-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9300-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9300-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9300-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9300-112">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b9300-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9300-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9300-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9300-114">Not supported.</span></span>    |
|<span data-ttu-id="b9300-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9300-115">Application</span></span> | <span data-ttu-id="b9300-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9300-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9300-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9300-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="b9300-118">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="b9300-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9300-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9300-119">Request headers</span></span>
| <span data-ttu-id="b9300-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b9300-120">Name</span></span>       | <span data-ttu-id="b9300-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b9300-121">Type</span></span> | <span data-ttu-id="b9300-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9300-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9300-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9300-123">Authorization</span></span>  | <span data-ttu-id="b9300-124">string</span><span class="sxs-lookup"><span data-stu-id="b9300-124">string</span></span>  | <span data-ttu-id="b9300-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9300-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9300-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9300-127">Request body</span></span>
<span data-ttu-id="b9300-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9300-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9300-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9300-129">Response</span></span>

<span data-ttu-id="b9300-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b9300-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9300-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b9300-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9300-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9300-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9300-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9300-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="b9300-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9300-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9300-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9300-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9300-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9300-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9300-138">Java</span><span class="sxs-lookup"><span data-stu-id="b9300-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9300-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9300-139">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

