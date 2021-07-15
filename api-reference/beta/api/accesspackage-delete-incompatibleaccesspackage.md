---
title: Удаление accessPackage из несовместимыхAccessPackages
description: Удалите ссылку, которая указывает, что пакет доступа несовместим с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c228402a433c3d9920481030ead07e79333459bc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439386"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="aef98-103">Удаление accessPackage из несовместимыхAccessPackages</span><span class="sxs-lookup"><span data-stu-id="aef98-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="aef98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aef98-105">Удаление пакета [доступа](../resources/accesspackage.md) из списка пакетов доступа, помеченных как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="aef98-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="aef98-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aef98-106">Permissions</span></span>

<span data-ttu-id="aef98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aef98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aef98-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aef98-109">Permission type</span></span>                        | <span data-ttu-id="aef98-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aef98-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aef98-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aef98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aef98-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef98-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="aef98-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aef98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aef98-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aef98-114">Not supported.</span></span> |
| <span data-ttu-id="aef98-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="aef98-115">Application</span></span>                            | <span data-ttu-id="aef98-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aef98-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aef98-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aef98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="aef98-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aef98-118">Request headers</span></span>

| <span data-ttu-id="aef98-119">Имя</span><span class="sxs-lookup"><span data-stu-id="aef98-119">Name</span></span>          | <span data-ttu-id="aef98-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aef98-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="aef98-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aef98-121">Authorization</span></span> | <span data-ttu-id="aef98-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef98-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aef98-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aef98-124">Content-Type</span></span>  | <span data-ttu-id="aef98-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aef98-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aef98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aef98-127">Request body</span></span>

<span data-ttu-id="aef98-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aef98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aef98-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef98-129">Response</span></span>

<span data-ttu-id="aef98-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="aef98-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aef98-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="aef98-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aef98-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="aef98-133">Request</span></span>

<span data-ttu-id="aef98-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aef98-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aef98-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aef98-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="aef98-136">C#</span><span class="sxs-lookup"><span data-stu-id="aef98-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-incompatibleaccesspackage-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aef98-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aef98-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-incompatibleaccesspackage-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aef98-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aef98-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-incompatibleaccesspackage-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aef98-139">Java</span><span class="sxs-lookup"><span data-stu-id="aef98-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-incompatibleaccesspackage-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="aef98-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="aef98-140">Response</span></span>

<span data-ttu-id="aef98-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aef98-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

