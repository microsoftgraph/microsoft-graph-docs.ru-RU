---
title: Получение Клаудпкдевицеимажес
description: Чтение свойств и связей объекта Клаудпкдевицеимаже.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: bb78a1eb6b6015ab7b32eb68fdaf4edc68f387e4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563326"
---
# <a name="get-cloudpcdeviceimage"></a><span data-ttu-id="48d90-103">Получение Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="48d90-103">Get cloudPcDeviceImage</span></span>

<span data-ttu-id="48d90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48d90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48d90-105">Чтение свойств и связей определенного объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="48d90-105">Read the properties and relationships of a specific [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="48d90-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48d90-106">Permissions</span></span>

<span data-ttu-id="48d90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48d90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48d90-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48d90-109">Permission type</span></span>|<span data-ttu-id="48d90-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48d90-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48d90-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48d90-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48d90-112">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="48d90-112">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="48d90-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48d90-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48d90-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48d90-114">Not supported.</span></span>|
|<span data-ttu-id="48d90-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48d90-115">Application</span></span>|<span data-ttu-id="48d90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48d90-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48d90-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48d90-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48d90-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48d90-118">Optional query parameters</span></span>

<span data-ttu-id="48d90-119">Этот метод поддерживает `$select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48d90-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="48d90-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="48d90-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="48d90-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48d90-121">Request headers</span></span>

| <span data-ttu-id="48d90-122">Имя</span><span class="sxs-lookup"><span data-stu-id="48d90-122">Name</span></span>          | <span data-ttu-id="48d90-123">Описание</span><span class="sxs-lookup"><span data-stu-id="48d90-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="48d90-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48d90-124">Authorization</span></span> | <span data-ttu-id="48d90-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48d90-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48d90-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48d90-127">Request body</span></span>

<span data-ttu-id="48d90-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48d90-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48d90-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="48d90-129">Response</span></span>

<span data-ttu-id="48d90-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48d90-130">If successful, this method returns a `200 OK` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48d90-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="48d90-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48d90-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="48d90-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="48d90-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="48d90-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[<span data-ttu-id="48d90-134">C#</span><span class="sxs-lookup"><span data-stu-id="48d90-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48d90-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48d90-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48d90-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48d90-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48d90-137">Java</span><span class="sxs-lookup"><span data-stu-id="48d90-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48d90-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="48d90-138">Response</span></span>

<span data-ttu-id="48d90-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48d90-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
    "id": "eda7ed64-7705-4079-9d08-c2bd883f4fff",
    "displayName": "Display Name value",
    "osBuildNumber": "OS Build Number value",
    "operatingSystem": "Operating System value",
    "version": "Version value",
    "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
    "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
    "status": "pending",
    "statusDetails": null
  }
}
```
