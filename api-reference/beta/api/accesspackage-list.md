---
title: Список Акцесспаккажес
description: Получение списка объектов Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 660eccde7211c23bfbb6ecc44faa20532934f965
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331117"
---
# <a name="list-accesspackages"></a><span data-ttu-id="b2fcc-103">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="b2fcc-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2fcc-104">Получение списка объектов [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="b2fcc-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="b2fcc-105">Полученный список включает все пакеты доступа, которые абонент имеет доступ для чтения, во всех каталогах.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2fcc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2fcc-106">Permissions</span></span>

<span data-ttu-id="b2fcc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2fcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2fcc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2fcc-109">Permission type</span></span>                        | <span data-ttu-id="b2fcc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2fcc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2fcc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2fcc-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b2fcc-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2fcc-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b2fcc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2fcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2fcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-114">Not supported.</span></span> |
| <span data-ttu-id="b2fcc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2fcc-115">Application</span></span>                            | <span data-ttu-id="b2fcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2fcc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2fcc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2fcc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2fcc-118">Optional query parameters</span></span>

<span data-ttu-id="b2fcc-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b2fcc-120">Например, чтобы получить политики пакетов доступа для каждого пакета Access, добавьте `$expand=accessPackageAssignmentPolicies`.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="b2fcc-121">Для поиска пакетов Access с определенным именем добавьте фильтр, например `$filter=contains(tolower(displayName),'team')` в запрос.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-121">To search for access packages with a particular name, include a filter such as `$filter=contains(tolower(displayName),'team')` in the query.</span></span> <span data-ttu-id="b2fcc-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b2fcc-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2fcc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2fcc-123">Request headers</span></span>

| <span data-ttu-id="b2fcc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b2fcc-124">Name</span></span>      |<span data-ttu-id="b2fcc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b2fcc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b2fcc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2fcc-126">Authorization</span></span> | <span data-ttu-id="b2fcc-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-127">Bearer \{token\}.</span></span> <span data-ttu-id="b2fcc-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2fcc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2fcc-129">Request body</span></span>

<span data-ttu-id="b2fcc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2fcc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2fcc-131">Response</span></span>

<span data-ttu-id="b2fcc-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2fcc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b2fcc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2fcc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2fcc-134">Request</span></span>

<span data-ttu-id="b2fcc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b2fcc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2fcc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="c"></a>[<span data-ttu-id="b2fcc-137">C#</span><span class="sxs-lookup"><span data-stu-id="b2fcc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2fcc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2fcc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2fcc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2fcc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2fcc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2fcc-140">Response</span></span>

<span data-ttu-id="b2fcc-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-141">The following is an example of the response.</span></span>

> <span data-ttu-id="b2fcc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2fcc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package",
      "displayName":"Access package for testing",
      "isHidden":false,
      "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
      "isRoleScopesVisible":false,
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
