---
title: Удаление Унифиедроледефинитион
description: Удаление объекта Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f2eab11e3683bd997bb2fa34999904865677e05
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43805934"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="10667-103">Удаление Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="10667-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="10667-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10667-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10667-105">Удаление объекта [унифиедроледефинитион](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="10667-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10667-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10667-106">Permissions</span></span>

<span data-ttu-id="10667-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10667-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10667-109">Permission type</span></span>                        | <span data-ttu-id="10667-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10667-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10667-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10667-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10667-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="10667-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="10667-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10667-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10667-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10667-114">Not supported.</span></span> |
| <span data-ttu-id="10667-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10667-115">Application</span></span>                            | <span data-ttu-id="10667-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="10667-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="10667-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10667-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="10667-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10667-118">Request headers</span></span>

| <span data-ttu-id="10667-119">Имя</span><span class="sxs-lookup"><span data-stu-id="10667-119">Name</span></span>          | <span data-ttu-id="10667-120">Описание</span><span class="sxs-lookup"><span data-stu-id="10667-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="10667-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10667-121">Authorization</span></span> | <span data-ttu-id="10667-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10667-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10667-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10667-123">Request body</span></span>

<span data-ttu-id="10667-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10667-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10667-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="10667-125">Response</span></span>

<span data-ttu-id="10667-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="10667-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10667-128">Пример</span><span class="sxs-lookup"><span data-stu-id="10667-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="10667-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="10667-129">Request</span></span>

<span data-ttu-id="10667-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10667-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10667-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="10667-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="10667-132">C#</span><span class="sxs-lookup"><span data-stu-id="10667-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10667-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10667-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10667-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10667-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10667-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="10667-135">Response</span></span>

<span data-ttu-id="10667-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10667-136">The following is an example of the response.</span></span>

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
