---
title: Список cloudPcProvisioningPolicy
description: Просмотр свойств и связей всех политик продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7d1090af54f82e730b20238ddb4e26c8e5a31de
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547648"
---
# <a name="list-provisioningpolicies"></a><span data-ttu-id="d8b0e-103">Список provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="d8b0e-103">List provisioningPolicies</span></span>

<span data-ttu-id="d8b0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8b0e-105">Список свойств и связей объектов [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d8b0e-105">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="d8b0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8b0e-106">Permissions</span></span>

<span data-ttu-id="d8b0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8b0e-109">Permission type</span></span>|<span data-ttu-id="d8b0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8b0e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8b0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8b0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8b0e-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b0e-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="d8b0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8b0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8b0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-114">Not supported.</span></span>|
|<span data-ttu-id="d8b0e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8b0e-115">Application</span></span>|<span data-ttu-id="d8b0e-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b0e-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8b0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8b0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8b0e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8b0e-118">Optional query parameters</span></span>

<span data-ttu-id="d8b0e-119">Этот метод поддерживает `$select` и `$filter` `$expand` параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-119">This method supports `$select`, `$filter` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="d8b0e-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d8b0e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8b0e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8b0e-121">Request headers</span></span>

| <span data-ttu-id="d8b0e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d8b0e-122">Name</span></span>          | <span data-ttu-id="d8b0e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d8b0e-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d8b0e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8b0e-124">Authorization</span></span> | <span data-ttu-id="d8b0e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8b0e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8b0e-127">Request body</span></span>

<span data-ttu-id="d8b0e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8b0e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8b0e-129">Response</span></span>

<span data-ttu-id="d8b0e-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8b0e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d8b0e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8b0e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8b0e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d8b0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8b0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcprovisioningpolicies"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
```
# <a name="c"></a>[<span data-ttu-id="d8b0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="d8b0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcprovisioningpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8b0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8b0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcprovisioningpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8b0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8b0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcprovisioningpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8b0e-137">Java</span><span class="sxs-lookup"><span data-stu-id="d8b0e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcprovisioningpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d8b0e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8b0e-138">Response</span></span>

<span data-ttu-id="d8b0e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8b0e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcProvisioningPolicy)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
      "id": "1d164206-bf41-4fd2-8424-a3192d392273",
      "displayName": "Display Name value",
      "description": "Description value",
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "imageId": "Image ID value",
      "imageDisplayName": "Image Display Name value",
      "imageType":"custom"
    }
  ]
}
```
