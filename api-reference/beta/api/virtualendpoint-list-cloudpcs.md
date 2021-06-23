---
title: CloudPCs списка
description: Список свойств и связей объектов cloudPC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 49cdea1b601e33210bc2861ee350086377fe05f8
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082386"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="14ff8-103">CloudPCs списка</span><span class="sxs-lookup"><span data-stu-id="14ff8-103">List cloudPCs</span></span>

<span data-ttu-id="14ff8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14ff8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14ff8-105">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="14ff8-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="14ff8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14ff8-106">Permissions</span></span>

<span data-ttu-id="14ff8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ff8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ff8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14ff8-109">Permission type</span></span>|<span data-ttu-id="14ff8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14ff8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14ff8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14ff8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14ff8-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ff8-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="14ff8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14ff8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14ff8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14ff8-114">Not supported.</span></span>|
|<span data-ttu-id="14ff8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="14ff8-115">Application</span></span>|<span data-ttu-id="14ff8-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ff8-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14ff8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14ff8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14ff8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14ff8-118">Optional query parameters</span></span>

<span data-ttu-id="14ff8-119">Этот метод поддерживает `$select` и `$filter` `$count` параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14ff8-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="14ff8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14ff8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14ff8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14ff8-121">Request headers</span></span>

| <span data-ttu-id="14ff8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="14ff8-122">Name</span></span>          | <span data-ttu-id="14ff8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14ff8-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="14ff8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14ff8-124">Authorization</span></span> | <span data-ttu-id="14ff8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14ff8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14ff8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14ff8-127">Request body</span></span>

<span data-ttu-id="14ff8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14ff8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ff8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ff8-129">Response</span></span>

<span data-ttu-id="14ff8-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [cloudPC](../resources/cloudpc.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14ff8-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14ff8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="14ff8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14ff8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="14ff8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="14ff8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="14ff8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="14ff8-134">C#</span><span class="sxs-lookup"><span data-stu-id="14ff8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14ff8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14ff8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14ff8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14ff8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14ff8-137">Java</span><span class="sxs-lookup"><span data-stu-id="14ff8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14ff8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ff8-138">Response</span></span>

<span data-ttu-id="14ff8-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="14ff8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPC)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPC",
      "id": "662009bc-7732-4f6f-8726-25883518ffff",
      "displayName": "Demo-1",
      "imageDisplayName": "Windows-10 19h1-evd",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "A00002GI001",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "provisioningPolicyName": "HR provisioning policy",
      "onPremisesConnectionName": "on-Premises connection for HR",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "pmitchell@cpccustomer001.onmicrosoft.com",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null,
      "gracePeriodEndDateTime": "2020-11-010T20:00:34Z"
    }
  ]
}
```
