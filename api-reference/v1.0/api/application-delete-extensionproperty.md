---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d9685a285ef82241ace355dd43d0b694b3816901
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999361"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="91ef5-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="91ef5-103">Delete extensionProperty</span></span>

<span data-ttu-id="91ef5-104">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="91ef5-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91ef5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91ef5-105">Permissions</span></span>

<span data-ttu-id="91ef5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91ef5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91ef5-108">Permission type</span></span>      | <span data-ttu-id="91ef5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91ef5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91ef5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91ef5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91ef5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91ef5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91ef5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91ef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91ef5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91ef5-113">Not supported.</span></span>    |
|<span data-ttu-id="91ef5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91ef5-114">Application</span></span> | <span data-ttu-id="91ef5-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91ef5-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91ef5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91ef5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91ef5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91ef5-117">Request headers</span></span>

| <span data-ttu-id="91ef5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="91ef5-118">Name</span></span>       | <span data-ttu-id="91ef5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="91ef5-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="91ef5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91ef5-120">Authorization</span></span>  | <span data-ttu-id="91ef5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91ef5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91ef5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91ef5-123">Request body</span></span>

<span data-ttu-id="91ef5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91ef5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91ef5-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="91ef5-125">Response</span></span>

<span data-ttu-id="91ef5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="91ef5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91ef5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="91ef5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91ef5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="91ef5-129">Request</span></span>

<span data-ttu-id="91ef5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91ef5-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91ef5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="91ef5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91ef5-132">C#</span><span class="sxs-lookup"><span data-stu-id="91ef5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91ef5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91ef5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91ef5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91ef5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="91ef5-135">Java</span><span class="sxs-lookup"><span data-stu-id="91ef5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-extensionproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91ef5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="91ef5-136">Response</span></span>

<span data-ttu-id="91ef5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91ef5-137">The following is an example of the response.</span></span>

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
  "description": "Delete extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
