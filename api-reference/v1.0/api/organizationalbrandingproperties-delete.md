---
title: Удаление organizationalBrandingProperties
description: Удаление организационных свойств.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c0137697c0908a4d344621a2656711f3b389c19a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682490"
---
# <a name="delete-organizationalbrandingproperties"></a><span data-ttu-id="73b57-103">Удаление organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="73b57-103">Delete organizationalBrandingProperties</span></span>

<span data-ttu-id="73b57-104">Удаление [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="73b57-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b57-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73b57-105">Permissions</span></span>

<span data-ttu-id="73b57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73b57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73b57-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73b57-108">Permission type</span></span>                        | <span data-ttu-id="73b57-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73b57-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73b57-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73b57-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="73b57-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b57-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="73b57-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73b57-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b57-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b57-113">Not supported.</span></span> |
| <span data-ttu-id="73b57-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73b57-114">Application</span></span>                            | <span data-ttu-id="73b57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b57-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b57-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73b57-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{tenant id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="73b57-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73b57-117">Request headers</span></span>

| <span data-ttu-id="73b57-118">Имя</span><span class="sxs-lookup"><span data-stu-id="73b57-118">Name</span></span>          | <span data-ttu-id="73b57-119">Описание</span><span class="sxs-lookup"><span data-stu-id="73b57-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="73b57-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73b57-120">Authorization</span></span> | <span data-ttu-id="73b57-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73b57-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73b57-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73b57-123">Request body</span></span>

<span data-ttu-id="73b57-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73b57-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b57-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="73b57-125">Response</span></span>

<span data-ttu-id="73b57-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="73b57-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73b57-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="73b57-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73b57-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="73b57-129">Request</span></span>

<span data-ttu-id="73b57-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73b57-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73b57-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="73b57-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_1"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="73b57-132">C#</span><span class="sxs-lookup"><span data-stu-id="73b57-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73b57-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73b57-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73b57-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73b57-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73b57-135">Java</span><span class="sxs-lookup"><span data-stu-id="73b57-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73b57-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="73b57-136">Response</span></span>

<span data-ttu-id="73b57-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73b57-137">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
