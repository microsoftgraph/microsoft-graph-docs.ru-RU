---
title: Список accessPackagesIncompatibleWith
description: Извлечение списка accesspackages, которые указывают, что их права доступа несовместимы с определенным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: def48d58dbbc757c6a248fe8dac40adff9372320
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439237"
---
# <a name="list-accesspackagesincompatiblewith"></a><span data-ttu-id="94b1e-103">Список accessPackagesIncompatibleWith</span><span class="sxs-lookup"><span data-stu-id="94b1e-103">List accessPackagesIncompatibleWith</span></span>

<span data-ttu-id="94b1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94b1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b1e-105">Извлечение списка объектов [accessPackage,](../resources/accesspackage.md) отмеченных указанным [accessPackage](../resources/accesspackage.md) как несовместимых.</span><span class="sxs-lookup"><span data-stu-id="94b1e-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have marked a specified [accessPackage](../resources/accesspackage.md) as incompatible.</span></span>

## <a name="permissions"></a><span data-ttu-id="94b1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94b1e-106">Permissions</span></span>

<span data-ttu-id="94b1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94b1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94b1e-109">Permission type</span></span>                        | <span data-ttu-id="94b1e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94b1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94b1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94b1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94b1e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b1e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="94b1e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94b1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b1e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b1e-114">Not supported.</span></span> |
| <span data-ttu-id="94b1e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="94b1e-115">Application</span></span>                            | <span data-ttu-id="94b1e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b1e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b1e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94b1e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/accessPackagesIncompatibleWith
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94b1e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94b1e-118">Optional query parameters</span></span>

<span data-ttu-id="94b1e-119">Этот метод поддерживает параметры запроса OData для прогона на стороне сервера с помощью большого отклика.</span><span class="sxs-lookup"><span data-stu-id="94b1e-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="94b1e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94b1e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94b1e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94b1e-121">Request headers</span></span>

| <span data-ttu-id="94b1e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="94b1e-122">Name</span></span>      |<span data-ttu-id="94b1e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94b1e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94b1e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94b1e-124">Authorization</span></span> | <span data-ttu-id="94b1e-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94b1e-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94b1e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94b1e-127">Request body</span></span>

<span data-ttu-id="94b1e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94b1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94b1e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b1e-129">Response</span></span>

<span data-ttu-id="94b1e-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessPackage](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94b1e-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94b1e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="94b1e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94b1e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94b1e-132">Request</span></span>

<span data-ttu-id="94b1e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94b1e-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94b1e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94b1e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesincompatiblewith"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith
```
# <a name="c"></a>[<span data-ttu-id="94b1e-135">C#</span><span class="sxs-lookup"><span data-stu-id="94b1e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagesincompatiblewith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94b1e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94b1e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagesincompatiblewith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94b1e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94b1e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagesincompatiblewith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94b1e-138">Java</span><span class="sxs-lookup"><span data-stu-id="94b1e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagesincompatiblewith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="94b1e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b1e-139">Response</span></span>

<span data-ttu-id="94b1e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94b1e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="94b1e-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94b1e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackagesIncompatibleWith",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


