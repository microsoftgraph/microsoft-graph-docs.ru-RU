---
title: Удаление Унифиедроледефинитион
description: Удаление объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e64dfdc90152675b18bda72cc17effc57e1df681
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461627"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="15660-103">Удаление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="15660-103">Delete unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15660-104">Удаление объекта [унифиедроледефинитион](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="15660-104">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="15660-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15660-105">Permissions</span></span>

<span data-ttu-id="15660-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15660-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15660-108">Permission type</span></span>                        | <span data-ttu-id="15660-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15660-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15660-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15660-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15660-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="15660-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="15660-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15660-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15660-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15660-113">Not supported.</span></span> |
| <span data-ttu-id="15660-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15660-114">Application</span></span>                            | <span data-ttu-id="15660-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="15660-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="15660-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15660-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="15660-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15660-117">Request headers</span></span>

| <span data-ttu-id="15660-118">Имя</span><span class="sxs-lookup"><span data-stu-id="15660-118">Name</span></span>          | <span data-ttu-id="15660-119">Описание</span><span class="sxs-lookup"><span data-stu-id="15660-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="15660-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15660-120">Authorization</span></span> | <span data-ttu-id="15660-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="15660-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="15660-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15660-122">Request body</span></span>

<span data-ttu-id="15660-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15660-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15660-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="15660-124">Response</span></span>

<span data-ttu-id="15660-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="15660-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15660-127">Пример</span><span class="sxs-lookup"><span data-stu-id="15660-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="15660-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="15660-128">Request</span></span>

<span data-ttu-id="15660-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15660-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15660-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="15660-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="15660-131">C#</span><span class="sxs-lookup"><span data-stu-id="15660-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15660-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15660-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15660-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="15660-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15660-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="15660-134">Response</span></span>

<span data-ttu-id="15660-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15660-135">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
