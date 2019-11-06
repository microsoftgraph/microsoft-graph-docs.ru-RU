---
title: Список Акцесспаккажес
description: Получение списка объектов Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c431216078d72a7515820e0c7ace5234cd08254f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994158"
---
# <a name="list-accesspackages"></a><span data-ttu-id="b5c09-103">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="b5c09-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c09-104">Получение списка объектов [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="b5c09-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="b5c09-105">Полученный список включает все пакеты доступа, которые абонент имеет доступ для чтения, во всех каталогах.</span><span class="sxs-lookup"><span data-stu-id="b5c09-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5c09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5c09-106">Permissions</span></span>

<span data-ttu-id="b5c09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5c09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5c09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5c09-109">Permission type</span></span>                        | <span data-ttu-id="b5c09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5c09-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5c09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5c09-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b5c09-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c09-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b5c09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5c09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5c09-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5c09-114">Not supported.</span></span> |
| <span data-ttu-id="b5c09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5c09-115">Application</span></span>                            | <span data-ttu-id="b5c09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5c09-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5c09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5c09-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5c09-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5c09-118">Optional query parameters</span></span>

<span data-ttu-id="b5c09-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5c09-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b5c09-120">Например, чтобы получить политики пакетов доступа для каждого пакета Access, добавьте `$expand=accessPackageAssignmentPolicies`.</span><span class="sxs-lookup"><span data-stu-id="b5c09-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="b5c09-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b5c09-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5c09-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5c09-122">Request headers</span></span>

| <span data-ttu-id="b5c09-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b5c09-123">Name</span></span>      |<span data-ttu-id="b5c09-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b5c09-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5c09-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5c09-125">Authorization</span></span> | <span data-ttu-id="b5c09-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="b5c09-126">Bearer \{token\}.</span></span> <span data-ttu-id="b5c09-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b5c09-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5c09-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5c09-128">Request body</span></span>

<span data-ttu-id="b5c09-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5c09-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5c09-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5c09-130">Response</span></span>

<span data-ttu-id="b5c09-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5c09-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5c09-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5c09-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b5c09-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5c09-133">Request</span></span>

<span data-ttu-id="b5c09-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5c09-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b5c09-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5c09-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5c09-136">C#</span><span class="sxs-lookup"><span data-stu-id="b5c09-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5c09-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5c09-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5c09-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5c09-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5c09-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5c09-139">Response</span></span>

<span data-ttu-id="b5c09-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5c09-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b5c09-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5c09-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
