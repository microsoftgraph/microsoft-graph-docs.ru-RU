---
title: Список ресурсов azureADDevice
description: Получите список объектов AzureADDevice и их свойств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 84c70d23b1b8bfadbc1820ea63a0589d972a4b40
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239297"
---
# <a name="list-azureaddevice-resources"></a><span data-ttu-id="5c41c-103">Список ресурсов azureADDevice</span><span class="sxs-lookup"><span data-stu-id="5c41c-103">List azureADDevice resources</span></span>
<span data-ttu-id="5c41c-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="5c41c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c41c-105">Получите список объектов [AzureADDevice](../resources/windowsupdates-azureaddevice.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5c41c-105">Get a list of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>

<span data-ttu-id="5c41c-106">Эта операция фильтрует полностью квалифицированный тип ресурса, который наследуется от `microsoft.graph.windowsUpdates.azureADDevice` [updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="5c41c-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.azureADDevice`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c41c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c41c-107">Permissions</span></span>
<span data-ttu-id="5c41c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c41c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c41c-110">Permission type</span></span>|<span data-ttu-id="5c41c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c41c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c41c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c41c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c41c-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c41c-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="5c41c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c41c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c41c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c41c-115">Not supported.</span></span>|
|<span data-ttu-id="5c41c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c41c-116">Application</span></span>|<span data-ttu-id="5c41c-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c41c-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c41c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c41c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c41c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c41c-119">Optional query parameters</span></span>
<span data-ttu-id="5c41c-120">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5c41c-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="5c41c-121">Чтобы использовать параметр запроса для свойства, которое не наследуется [от updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="5c41c-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="5c41c-122">Например, чтобы выбрать свойство **ошибок,** используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="5c41c-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c41c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c41c-123">Request headers</span></span>
|<span data-ttu-id="5c41c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5c41c-124">Name</span></span>|<span data-ttu-id="5c41c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5c41c-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c41c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c41c-126">Authorization</span></span>|<span data-ttu-id="5c41c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c41c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c41c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c41c-129">Request body</span></span>
<span data-ttu-id="5c41c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c41c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c41c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c41c-131">Response</span></span>

<span data-ttu-id="5c41c-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [azureADDevice](../resources/windowsupdates-azureaddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c41c-132">If successful, this method returns a `200 OK` response code and a collection of [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c41c-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c41c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c41c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c41c-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5c41c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c41c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.azureADDevice')
```
# <a name="c"></a>[<span data-ttu-id="5c41c-136">C#</span><span class="sxs-lookup"><span data-stu-id="5c41c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c41c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c41c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c41c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c41c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c41c-139">Java</span><span class="sxs-lookup"><span data-stu-id="5c41c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c41c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c41c-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.azureADDevice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
      "errors": [],
      "enrollments": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
          "updateCategory": "feature"
        }
      ]
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "90b91efa-6d46-42cd-ad4d-381831773a85",
      "errors": [],
      "enrollments": []
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "0ee3eb63-caf3-44ce-9769-b83188cc683d",
      "errors": [
        {
          "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
        }
      ],
      "enrollments": []
    }
  ]
}
```

