---
title: Удаление Екстенсионпроперти
description: Удаление Екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a391295573ba6b0c2949aef357311e7043f62f40
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006440"
---
# <a name="delete-extensionproperty"></a><span data-ttu-id="2ada3-103">Удаление Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="2ada3-103">Delete extensionProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ada3-104">Удаление [екстенсионпроперти](../resources/extensionproperty.md).</span><span class="sxs-lookup"><span data-stu-id="2ada3-104">Delete an [extensionProperty](../resources/extensionproperty.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ada3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ada3-105">Permissions</span></span>

<span data-ttu-id="2ada3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ada3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ada3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ada3-108">Permission type</span></span>      | <span data-ttu-id="2ada3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ada3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ada3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ada3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ada3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ada3-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ada3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ada3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ada3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ada3-113">Not supported.</span></span>    |
|<span data-ttu-id="2ada3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ada3-114">Application</span></span> | <span data-ttu-id="2ada3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ada3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ada3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ada3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/extensionProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ada3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ada3-117">Request headers</span></span>

| <span data-ttu-id="2ada3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2ada3-118">Name</span></span>       | <span data-ttu-id="2ada3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2ada3-119">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="2ada3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ada3-120">Authorization</span></span>  | <span data-ttu-id="2ada3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ada3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ada3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ada3-123">Request body</span></span>

<span data-ttu-id="2ada3-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ada3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ada3-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ada3-125">Response</span></span>

<span data-ttu-id="2ada3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ada3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ada3-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ada3-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ada3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ada3-129">Request</span></span>

<span data-ttu-id="2ada3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ada3-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ada3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ada3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_extensionproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/extensionProperties/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ada3-132">C#</span><span class="sxs-lookup"><span data-stu-id="2ada3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-extensionproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ada3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ada3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-extensionproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ada3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ada3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-extensionproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ada3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ada3-135">Response</span></span>

<span data-ttu-id="2ada3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ada3-136">The following is an example of the response.</span></span>

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