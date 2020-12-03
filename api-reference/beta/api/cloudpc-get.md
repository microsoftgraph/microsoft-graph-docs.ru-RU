---
title: Получение Клаудпкс
description: Просмотр свойств и связей объекта Клаудпк.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7c4773fd15528f4c8548b2714959b5e169d42651
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563417"
---
# <a name="get-cloudpc"></a><span data-ttu-id="a34b8-103">Получение Клаудпк</span><span class="sxs-lookup"><span data-stu-id="a34b8-103">Get cloudPC</span></span>

<span data-ttu-id="a34b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a34b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a34b8-105">Чтение свойств и связей определенного объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="a34b8-105">Read the properties and relationships of a specific [cloudPC](../resources/cloudpc.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="a34b8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a34b8-106">Permissions</span></span>

<span data-ttu-id="a34b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a34b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a34b8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a34b8-109">Permission type</span></span>|<span data-ttu-id="a34b8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a34b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a34b8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a34b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a34b8-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a34b8-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="a34b8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a34b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a34b8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34b8-114">Not supported.</span></span>|
|<span data-ttu-id="a34b8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a34b8-115">Application</span></span>|<span data-ttu-id="a34b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a34b8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a34b8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/cloudPCs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a34b8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a34b8-118">Optional query parameters</span></span>

<span data-ttu-id="a34b8-119">Этот метод поддерживает `$select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a34b8-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="a34b8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a34b8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a34b8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a34b8-121">Request headers</span></span>

| <span data-ttu-id="a34b8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a34b8-122">Name</span></span>          | <span data-ttu-id="a34b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a34b8-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a34b8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a34b8-124">Authorization</span></span> | <span data-ttu-id="a34b8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a34b8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a34b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a34b8-127">Request body</span></span>

<span data-ttu-id="a34b8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a34b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a34b8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a34b8-129">Response</span></span>

<span data-ttu-id="a34b8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпк](../resources/cloudpc.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a34b8-130">If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a34b8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a34b8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a34b8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a34b8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a34b8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a34b8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{id}
```
# <a name="c"></a>[<span data-ttu-id="a34b8-134">C#</span><span class="sxs-lookup"><span data-stu-id="a34b8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a34b8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a34b8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a34b8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a34b8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a34b8-137">Java</span><span class="sxs-lookup"><span data-stu-id="a34b8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a34b8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a34b8-138">Response</span></span>

<span data-ttu-id="a34b8-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a34b8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_cloudpc",
  "@odata.type": "microsoft.graph.cloudPC"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPC",
    "id": "ac74ae8b-85f7-4272-88cc-54192674ffff",
    "displayName": "Display Name value",
    "imageDisplayName": "Image Display Name value",
    "managedDeviceId": "e87f50c7-fa7f-4687-aade-dd45f3d6ffff",  
    "managedDeviceName": "Device Name value",
    "provisioningPolicyId": "13fa0778-ba00-438a-96d3-488c8602ffff",
    "servicePlanId": "da5615b4-a484-4742-a019-2d52c91cffff",
    "servicePlanName": "standard",
    "status": "failed",
    "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails",
    "code": "Sample code",
    "message": "Sample message",
    "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Sample value"
        }
      ]
    },
    "userPrincipalName": "User Principal Name value",
    "lastModifiedDateTime": "2020-11-03T18:14:34Z"
  }
}
```
