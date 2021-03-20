---
title: Удаление локализованных организационных свойствBrandingProperties
description: Удаление организационных свойств для определенной локализации.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 938a45dfe29d9473d57571f7b10e5693d8d8de05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943860"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="d8019-103">Удаление локализованных организационных свойствBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d8019-103">Delete Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8019-104">Удаление [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="d8019-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8019-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8019-105">Permissions</span></span>

<span data-ttu-id="d8019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8019-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8019-108">Permission type</span></span>                        | <span data-ttu-id="d8019-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8019-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d8019-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8019-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8019-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8019-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="d8019-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8019-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8019-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8019-113">Not supported.</span></span> |
| <span data-ttu-id="d8019-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8019-114">Application</span></span>                            | <span data-ttu-id="d8019-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8019-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8019-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8019-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="d8019-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8019-117">Request headers</span></span>

| <span data-ttu-id="d8019-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d8019-118">Name</span></span>          | <span data-ttu-id="d8019-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d8019-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d8019-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8019-120">Authorization</span></span> | <span data-ttu-id="d8019-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8019-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8019-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8019-123">Request body</span></span>

<span data-ttu-id="d8019-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8019-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8019-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8019-125">Response</span></span>

<span data-ttu-id="d8019-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d8019-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8019-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d8019-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8019-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8019-129">Request</span></span>

<span data-ttu-id="d8019-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8019-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8019-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8019-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="d8019-132">C#</span><span class="sxs-lookup"><span data-stu-id="d8019-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8019-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8019-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8019-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8019-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8019-135">Java</span><span class="sxs-lookup"><span data-stu-id="d8019-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d8019-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8019-136">Response</span></span>

<span data-ttu-id="d8019-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8019-137">The following is an example of the response.</span></span>

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
