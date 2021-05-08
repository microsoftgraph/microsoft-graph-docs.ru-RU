---
title: Get azureADDevice
description: Ознакомьтесь с свойствами объекта azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 480940d2b0b13ff32b002d5a1ff4a5922d9db29c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241103"
---
# <a name="get-azureaddevice"></a><span data-ttu-id="a5bd4-103">Get azureADDevice</span><span class="sxs-lookup"><span data-stu-id="a5bd4-103">Get azureADDevice</span></span>
<span data-ttu-id="a5bd4-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a5bd4-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5bd4-105">Ознакомьтесь с свойствами объекта [azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a5bd4-105">Read the properties of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5bd4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5bd4-106">Permissions</span></span>
<span data-ttu-id="a5bd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5bd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5bd4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5bd4-109">Permission type</span></span>|<span data-ttu-id="a5bd4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5bd4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5bd4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5bd4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5bd4-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bd4-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="a5bd4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5bd4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5bd4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-114">Not supported.</span></span>|
|<span data-ttu-id="a5bd4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5bd4-115">Application</span></span>|<span data-ttu-id="a5bd4-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bd4-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5bd4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5bd4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{azureADDeviceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5bd4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a5bd4-118">Optional query parameters</span></span>
<span data-ttu-id="a5bd4-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a5bd4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a5bd4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="a5bd4-121">Чтобы использовать параметр запроса для свойства, которое не наследуется [от updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-121">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type.</span></span> <span data-ttu-id="a5bd4-122">Например, чтобы выбрать свойство **ошибок,** используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="a5bd4-122">For example, to select the **errors** property, use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5bd4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5bd4-123">Request headers</span></span>
|<span data-ttu-id="a5bd4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a5bd4-124">Name</span></span>|<span data-ttu-id="a5bd4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a5bd4-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a5bd4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5bd4-126">Authorization</span></span>|<span data-ttu-id="a5bd4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5bd4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5bd4-129">Request body</span></span>
<span data-ttu-id="a5bd4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5bd4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5bd4-131">Response</span></span>

<span data-ttu-id="a5bd4-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект azureADDevice](../resources/windowsupdates-azureaddevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5bd4-132">If successful, this method returns a `200 OK` response code and an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5bd4-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5bd4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5bd4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5bd4-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a5bd4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bd4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_azureaddevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```
# <a name="c"></a>[<span data-ttu-id="a5bd4-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5bd4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-azureaddevice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5bd4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5bd4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-azureaddevice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5bd4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5bd4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-azureaddevice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5bd4-139">Java</span><span class="sxs-lookup"><span data-stu-id="a5bd4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-azureaddevice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5bd4-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5bd4-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

