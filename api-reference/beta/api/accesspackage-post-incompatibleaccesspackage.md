---
title: Добавление accessPackage в несовместимыеAccessPackages
description: Добавьте ссылку, чтобы указать, что пакет доступа несовместим с указанным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4ddb6953346a5ea571a480dc073e29dca14cca31
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439844"
---
# <a name="add-accesspackage-to-incompatibleaccesspackages"></a><span data-ttu-id="56d26-103">Добавление accessPackage в несовместимыеAccessPackages</span><span class="sxs-lookup"><span data-stu-id="56d26-103">Add accessPackage to incompatibleAccessPackages</span></span>

<span data-ttu-id="56d26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56d26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56d26-105">Добавьте [accessPackage в](../resources/accesspackage.md) список пакетов доступа, которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="56d26-105">Add an [accessPackage](../resources/accesspackage.md) to the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="56d26-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56d26-106">Permissions</span></span>

<span data-ttu-id="56d26-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56d26-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56d26-109">Permission type</span></span>                        | <span data-ttu-id="56d26-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56d26-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56d26-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56d26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="56d26-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d26-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="56d26-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56d26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d26-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d26-114">Not supported.</span></span> |
| <span data-ttu-id="56d26-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="56d26-115">Application</span></span>                            | <span data-ttu-id="56d26-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d26-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d26-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56d26-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
```

## <a name="request-headers"></a><span data-ttu-id="56d26-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56d26-118">Request headers</span></span>

| <span data-ttu-id="56d26-119">Имя</span><span class="sxs-lookup"><span data-stu-id="56d26-119">Name</span></span>          | <span data-ttu-id="56d26-120">Описание</span><span class="sxs-lookup"><span data-stu-id="56d26-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="56d26-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56d26-121">Authorization</span></span> | <span data-ttu-id="56d26-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56d26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56d26-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56d26-124">Content-Type</span></span>  | <span data-ttu-id="56d26-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56d26-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56d26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56d26-127">Request body</span></span>

<span data-ttu-id="56d26-128">В теле запроса поставляем JSON представление структуры с IData id URI объекта [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="56d26-128">In the request body, supply a JSON representation of a structure with the OData id of the URI of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="56d26-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d26-129">Response</span></span>

<span data-ttu-id="56d26-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="56d26-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56d26-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="56d26-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56d26-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="56d26-133">Request</span></span>

<span data-ttu-id="56d26-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56d26-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="56d26-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="56d26-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_incompatibleaccesspackage_to_accesspackage"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
Content-type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}
```
# <a name="c"></a>[<span data-ttu-id="56d26-136">C#</span><span class="sxs-lookup"><span data-stu-id="56d26-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-incompatibleaccesspackage-to-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56d26-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56d26-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-incompatibleaccesspackage-to-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56d26-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56d26-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-incompatibleaccesspackage-to-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="56d26-139">Java</span><span class="sxs-lookup"><span data-stu-id="56d26-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-incompatibleaccesspackage-to-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56d26-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="56d26-140">Response</span></span>

<span data-ttu-id="56d26-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56d26-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Created
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

