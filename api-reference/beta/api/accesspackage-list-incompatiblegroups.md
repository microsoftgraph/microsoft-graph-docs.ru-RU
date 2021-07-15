---
title: Несовместимые группы списка
description: Извлечение списка групп, права доступа которых несовместимы с определенным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c5af81b8995b0fc0662a35157ab4579631b5f189
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439928"
---
# <a name="list-incompatiblegroups"></a><span data-ttu-id="eb771-103">Несовместимые группы списка</span><span class="sxs-lookup"><span data-stu-id="eb771-103">List incompatibleGroups</span></span>

<span data-ttu-id="eb771-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb771-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb771-105">Извлечение списка [объектов группы,](../resources/group.md) которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="eb771-105">Retrieve a list of the [group](../resources/group.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="eb771-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb771-106">Permissions</span></span>

<span data-ttu-id="eb771-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb771-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb771-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb771-109">Permission type</span></span>                        | <span data-ttu-id="eb771-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb771-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eb771-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb771-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb771-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb771-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="eb771-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb771-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb771-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb771-114">Not supported.</span></span> |
| <span data-ttu-id="eb771-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="eb771-115">Application</span></span>                            | <span data-ttu-id="eb771-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb771-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb771-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb771-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb771-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb771-118">Optional query parameters</span></span>

<span data-ttu-id="eb771-119">Этот метод поддерживает параметры запроса OData для прогона на стороне сервера с помощью большого отклика.</span><span class="sxs-lookup"><span data-stu-id="eb771-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="eb771-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eb771-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb771-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb771-121">Request headers</span></span>

| <span data-ttu-id="eb771-122">Имя</span><span class="sxs-lookup"><span data-stu-id="eb771-122">Name</span></span>      |<span data-ttu-id="eb771-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eb771-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb771-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb771-124">Authorization</span></span> | <span data-ttu-id="eb771-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb771-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb771-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb771-127">Request body</span></span>

<span data-ttu-id="eb771-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb771-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb771-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb771-129">Response</span></span>

<span data-ttu-id="eb771-130">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="eb771-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb771-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb771-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb771-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb771-132">Request</span></span>

<span data-ttu-id="eb771-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb771-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb771-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb771-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_incompatiblegroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups
```
# <a name="c"></a>[<span data-ttu-id="eb771-135">C#</span><span class="sxs-lookup"><span data-stu-id="eb771-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-incompatiblegroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb771-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb771-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-incompatiblegroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb771-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb771-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-incompatiblegroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb771-138">Java</span><span class="sxs-lookup"><span data-stu-id="eb771-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-incompatiblegroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb771-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb771-139">Response</span></span>

<span data-ttu-id="eb771-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eb771-140">The following is an example of the response.</span></span>

> <span data-ttu-id="eb771-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eb771-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "a743348f-5667-41a4-89a3-5ad8a94da5d2",
      "displayName": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

