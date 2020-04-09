---
title: Список Публишедресаурцес
description: Получение списка объектов Публишедресаурце.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d820e23e48eac46feb82e1304e5dffcf83e5d032
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200287"
---
# <a name="list-publishedresources"></a><span data-ttu-id="258b3-103">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="258b3-103">List publishedResources</span></span>

<span data-ttu-id="258b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="258b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="258b3-105">Получение списка объектов [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="258b3-105">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="258b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="258b3-106">Permissions</span></span>

<span data-ttu-id="258b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="258b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="258b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="258b3-109">Permission type</span></span>                        | <span data-ttu-id="258b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="258b3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="258b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="258b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="258b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258b3-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="258b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="258b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="258b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="258b3-114">Not supported.</span></span> |
| <span data-ttu-id="258b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="258b3-115">Application</span></span>                            | <span data-ttu-id="258b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="258b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="258b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="258b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="258b3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="258b3-118">Optional query parameters</span></span>

<span data-ttu-id="258b3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="258b3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="258b3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="258b3-120">Request headers</span></span>

| <span data-ttu-id="258b3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="258b3-121">Name</span></span>      |<span data-ttu-id="258b3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="258b3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="258b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="258b3-123">Authorization</span></span> | <span data-ttu-id="258b3-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="258b3-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="258b3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="258b3-125">Request body</span></span>

<span data-ttu-id="258b3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="258b3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="258b3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="258b3-127">Response</span></span>

<span data-ttu-id="258b3-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="258b3-128">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="258b3-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="258b3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="258b3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="258b3-130">Request</span></span>

<span data-ttu-id="258b3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="258b3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="258b3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="258b3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="258b3-133">C#</span><span class="sxs-lookup"><span data-stu-id="258b3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="258b3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="258b3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="258b3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="258b3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="258b3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="258b3-136">Response</span></span>

<span data-ttu-id="258b3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="258b3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="258b3-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="258b3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "publishingType": "provisioning",
      "displayName": "Demo provisioning",
      "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
      "resourceName": "domain1.contoso.com",
      "agentGroups": [
          {
              "id": "2d55ed41-1619-4848-92bb-0576d3038682",
              "displayName": "Group 1"
          }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List publishedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
