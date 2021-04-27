---
title: Создание accessPackage
description: Создание нового accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e6f6a80316bbdf12792bb47078be7f4e3ca9b48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048647"
---
# <a name="create-accesspackage"></a><span data-ttu-id="0cdb5-103">Создание accessPackage</span><span class="sxs-lookup"><span data-stu-id="0cdb5-103">Create accessPackage</span></span>

<span data-ttu-id="0cdb5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cdb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cdb5-105">Создайте новый [объект accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="0cdb5-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cdb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0cdb5-106">Permissions</span></span>

<span data-ttu-id="0cdb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cdb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0cdb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cdb5-109">Permission type</span></span>                        | <span data-ttu-id="0cdb5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cdb5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0cdb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cdb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cdb5-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cdb5-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0cdb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cdb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cdb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-114">Not supported.</span></span> |
| <span data-ttu-id="0cdb5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0cdb5-115">Application</span></span>                            | <span data-ttu-id="0cdb5-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cdb5-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cdb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cdb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="0cdb5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cdb5-118">Request headers</span></span>

| <span data-ttu-id="0cdb5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0cdb5-119">Name</span></span>          | <span data-ttu-id="0cdb5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0cdb5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0cdb5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cdb5-121">Authorization</span></span> | <span data-ttu-id="0cdb5-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="0cdb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cdb5-124">Content-Type</span></span>  | <span data-ttu-id="0cdb5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cdb5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cdb5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cdb5-126">Request body</span></span>

<span data-ttu-id="0cdb5-127">В теле запроса поставляем JSON-представление [объекта accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="0cdb5-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0cdb5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cdb5-128">Response</span></span>

<span data-ttu-id="0cdb5-129">В случае успешной работы этот метод возвращает созданный код ответа 201 и новый [объект accessPackage](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0cdb5-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0cdb5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0cdb5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cdb5-131">Request</span></span>

<span data-ttu-id="0cdb5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cdb5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cdb5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```
# <a name="c"></a>[<span data-ttu-id="0cdb5-134">C#</span><span class="sxs-lookup"><span data-stu-id="0cdb5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cdb5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cdb5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cdb5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cdb5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cdb5-137">Java</span><span class="sxs-lookup"><span data-stu-id="0cdb5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cdb5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cdb5-138">Response</span></span>

<span data-ttu-id="0cdb5-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="0cdb5-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0cdb5-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


