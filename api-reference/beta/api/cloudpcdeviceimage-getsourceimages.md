---
title: 'cloudPcDeviceImage: getSourceImages'
description: Просмотреть список всех ресурсов управляемых изображений из подписок Azure. Эти исходные изображения можно загрузить и использовать на облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1ddd7fdef827328f6f72b52af5a992e9f0d69653
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872781"
---
# <a name="cloudpcdeviceimage-getsourceimages"></a><span data-ttu-id="fb80b-104">cloudPcDeviceImage: getSourceImages</span><span class="sxs-lookup"><span data-stu-id="fb80b-104">cloudPcDeviceImage: getSourceImages</span></span>

<span data-ttu-id="fb80b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb80b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb80b-106">Получите [объекты cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="fb80b-106">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span> <span data-ttu-id="fb80b-107">Просмотреть список всех ресурсов управляемых изображений из подписок Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fb80b-107">View a list of all the managed image resources from your Azure Active Directory subscriptions.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="fb80b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb80b-108">Permissions</span></span>

<span data-ttu-id="fb80b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb80b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb80b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb80b-111">Permission type</span></span>|<span data-ttu-id="fb80b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb80b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb80b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb80b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb80b-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb80b-114">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb80b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb80b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb80b-116">Not supported.</span></span>|
|<span data-ttu-id="fb80b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb80b-117">Application</span></span>|<span data-ttu-id="fb80b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb80b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb80b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb80b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```

## <a name="request-headers"></a><span data-ttu-id="fb80b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb80b-120">Request headers</span></span>

|<span data-ttu-id="fb80b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fb80b-121">Name</span></span>|<span data-ttu-id="fb80b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb80b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fb80b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb80b-123">Authorization</span></span>|<span data-ttu-id="fb80b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb80b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb80b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb80b-126">Request body</span></span>

<span data-ttu-id="fb80b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb80b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb80b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb80b-128">Response</span></span>

<span data-ttu-id="fb80b-129">В случае успеха эта функция возвращает код отклика и коллекцию `200 OK` [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb80b-129">If successful, this function returns a `200 OK` response code and a [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb80b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb80b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb80b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb80b-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb80b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb80b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcdeviceimage_getsourceimages"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/getSourceImages
```
# <a name="c"></a>[<span data-ttu-id="fb80b-133">C#</span><span class="sxs-lookup"><span data-stu-id="fb80b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcdeviceimage-getsourceimages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb80b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb80b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcdeviceimage-getsourceimages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb80b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb80b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcdeviceimage-getsourceimages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb80b-136">Java</span><span class="sxs-lookup"><span data-stu-id="fb80b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcdeviceimage-getsourceimages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb80b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb80b-137">Response</span></span>

<span data-ttu-id="fb80b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fb80b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.cloudPcSourceDeviceImage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
      "id": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Compute/images/ExampleImage",
      "displayName": "Display Name value"
    }
  ]
}
```
