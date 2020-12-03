---
title: Список Клаудпкс
description: Список свойств и связей объектов Клаудпк.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 80fe8d0f8850acc7da90f44b7f6a96eb89c2d785
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563909"
---
# <a name="list-cloudpcs"></a><span data-ttu-id="ed3cc-103">Список Клаудпкс</span><span class="sxs-lookup"><span data-stu-id="ed3cc-103">List cloudPCs</span></span>

<span data-ttu-id="ed3cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed3cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed3cc-105">Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="ed3cc-105">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ed3cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed3cc-106">Permissions</span></span>

<span data-ttu-id="ed3cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed3cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed3cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed3cc-109">Permission type</span></span>|<span data-ttu-id="ed3cc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed3cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed3cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed3cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed3cc-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ed3cc-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="ed3cc-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed3cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed3cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-114">Not supported.</span></span>|
|<span data-ttu-id="ed3cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed3cc-115">Application</span></span>|<span data-ttu-id="ed3cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed3cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed3cc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed3cc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed3cc-118">Optional query parameters</span></span>

<span data-ttu-id="ed3cc-119">Этот метод поддерживает `$select` `$filter` и `$count` параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-119">This method supports `$select`, `$filter` and `$count` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed3cc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ed3cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed3cc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed3cc-121">Request headers</span></span>

| <span data-ttu-id="ed3cc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ed3cc-122">Name</span></span>          | <span data-ttu-id="ed3cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ed3cc-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ed3cc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed3cc-124">Authorization</span></span> | <span data-ttu-id="ed3cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed3cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed3cc-127">Request body</span></span>

<span data-ttu-id="ed3cc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed3cc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed3cc-129">Response</span></span>

<span data-ttu-id="ed3cc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаудпк](../resources/cloudpc.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-130">If successful, this method returns a `200 OK` response code and a collection of [cloudPC](../resources/cloudpc.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed3cc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed3cc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed3cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed3cc-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed3cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed3cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcs"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs
```
# <a name="c"></a>[<span data-ttu-id="ed3cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="ed3cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed3cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed3cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed3cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed3cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed3cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="ed3cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed3cc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed3cc-138">Response</span></span>

<span data-ttu-id="ed3cc-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ed3cc-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName": "Display Name value",
      "imageDisplayName": "Image Display Name value",
      "managedDeviceId": "bdc8e6dd-0455-4412-83d9-c818664fffff",
      "managedDeviceName": "Managed Device Name value",
      "provisioningPolicyId": "7ed725ad-0a00-4117-b557-d965c373ffff",
      "servicePlanId": "dbb9148c-ff83-4a4c-8d7f-28752e93ffff",
      "servicePlanName": "lite",
      "status": "provisioned",
      "userPrincipalName": "User Principal Name value",
      "lastModifiedDateTime": "2020-11-03T10:29:57Z",
      "statusDetails": null
    }
  ]
}
```
