---
title: Список Акцесспаккажересаурцес
description: Получение списка объектов акцесспаккажересаурце.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 726fdf04818717167b9909f02b43f3e333636e28
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441979"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="dfc9e-103">Список Акцесспаккажересаурцес</span><span class="sxs-lookup"><span data-stu-id="dfc9e-103">List accessPackageResources</span></span>

<span data-ttu-id="dfc9e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dfc9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfc9e-105">Получение списка объектов [акцесспаккажересаурце](../resources/accesspackageresource.md) в [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="dfc9e-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfc9e-106">Permissions</span></span>

<span data-ttu-id="dfc9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfc9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfc9e-109">Permission type</span></span>                        | <span data-ttu-id="dfc9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfc9e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfc9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfc9e-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="dfc9e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc9e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="dfc9e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfc9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-114">Not supported.</span></span> |
| <span data-ttu-id="dfc9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfc9e-115">Application</span></span>                            | <span data-ttu-id="dfc9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfc9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfc9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfc9e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfc9e-118">Optional query parameters</span></span>

<span data-ttu-id="dfc9e-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dfc9e-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dfc9e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfc9e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfc9e-121">Request headers</span></span>

| <span data-ttu-id="dfc9e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dfc9e-122">Name</span></span>      |<span data-ttu-id="dfc9e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc9e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfc9e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfc9e-124">Authorization</span></span> | <span data-ttu-id="dfc9e-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-125">Bearer \{token\}.</span></span> <span data-ttu-id="dfc9e-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfc9e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfc9e-127">Request body</span></span>

<span data-ttu-id="dfc9e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc9e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfc9e-129">Response</span></span>

<span data-ttu-id="dfc9e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурце](../resources/accesspackageresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfc9e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="dfc9e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfc9e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfc9e-132">Request</span></span>

<span data-ttu-id="dfc9e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfc9e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc9e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="dfc9e-135">C#</span><span class="sxs-lookup"><span data-stu-id="dfc9e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc9e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc9e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc9e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc9e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dfc9e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfc9e-138">Response</span></span>

<span data-ttu-id="dfc9e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dfc9e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfc9e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
