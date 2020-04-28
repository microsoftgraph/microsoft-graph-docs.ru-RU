---
title: Список Акцесспаккажес
description: Получение списка объектов Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3648320f1928eb6054970c92e9109ebac792d507
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448524"
---
# <a name="list-accesspackages"></a><span data-ttu-id="1a150-103">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="1a150-103">List accessPackages</span></span>

<span data-ttu-id="1a150-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a150-105">Получение списка объектов [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="1a150-105">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="1a150-106">Полученный список включает все пакеты доступа, которые абонент имеет доступ для чтения, во всех каталогах.</span><span class="sxs-lookup"><span data-stu-id="1a150-106">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a150-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a150-107">Permissions</span></span>

<span data-ttu-id="1a150-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a150-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a150-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a150-110">Permission type</span></span>                        | <span data-ttu-id="1a150-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a150-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a150-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a150-112">Delegated (work or school account)</span></span>     |  <span data-ttu-id="1a150-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a150-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1a150-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a150-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a150-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a150-115">Not supported.</span></span> |
| <span data-ttu-id="1a150-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a150-116">Application</span></span>                            | <span data-ttu-id="1a150-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a150-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a150-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a150-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a150-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a150-119">Optional query parameters</span></span>

<span data-ttu-id="1a150-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a150-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1a150-121">Например, чтобы получить политики пакетов доступа для каждого пакета Access, добавьте `$expand=accessPackageAssignmentPolicies`.</span><span class="sxs-lookup"><span data-stu-id="1a150-121">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="1a150-122">Для поиска пакетов Access с определенным именем добавьте фильтр, например `$filter=contains(tolower(displayName),'team')` в запрос.</span><span class="sxs-lookup"><span data-stu-id="1a150-122">To search for access packages with a particular name, include a filter such as `$filter=contains(tolower(displayName),'team')` in the query.</span></span> <span data-ttu-id="1a150-123">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1a150-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a150-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a150-124">Request headers</span></span>

| <span data-ttu-id="1a150-125">Имя</span><span class="sxs-lookup"><span data-stu-id="1a150-125">Name</span></span>      |<span data-ttu-id="1a150-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1a150-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a150-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a150-127">Authorization</span></span> | <span data-ttu-id="1a150-128">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="1a150-128">Bearer \{token\}.</span></span> <span data-ttu-id="1a150-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1a150-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a150-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a150-130">Request body</span></span>

<span data-ttu-id="1a150-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a150-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a150-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a150-132">Response</span></span>

<span data-ttu-id="1a150-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a150-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a150-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a150-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a150-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a150-135">Request</span></span>

<span data-ttu-id="1a150-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a150-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a150-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a150-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="c"></a>[<span data-ttu-id="1a150-138">C#</span><span class="sxs-lookup"><span data-stu-id="1a150-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a150-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a150-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a150-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a150-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a150-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a150-141">Response</span></span>

<span data-ttu-id="1a150-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a150-142">The following is an example of the response.</span></span>

> <span data-ttu-id="1a150-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a150-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
