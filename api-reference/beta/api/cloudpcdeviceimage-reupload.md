---
title: 'cloudPcDeviceImage: перезагрузка'
description: Перезагрузите объект cloudPcDeviceImage.
author: RuiHou105
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 8e359f749f0b932f3061bf8750fcf7992fe23302
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439494"
---
# <a name="cloudpcdeviceimage-reupload"></a><span data-ttu-id="ce9fc-103">cloudPcDeviceImage: перезагрузка</span><span class="sxs-lookup"><span data-stu-id="ce9fc-103">cloudPcDeviceImage: reupload</span></span>

<span data-ttu-id="ce9fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce9fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce9fc-105">Перезагрузите [объект cloudPcDeviceImage,](../resources/cloudpcdeviceimage.md) который не удалось загрузить.</span><span class="sxs-lookup"><span data-stu-id="ce9fc-105">Reupload a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object that failed to upload.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="permissions"></a><span data-ttu-id="ce9fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce9fc-106">Permissions</span></span>

<span data-ttu-id="ce9fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce9fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce9fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce9fc-109">Permission type</span></span>|<span data-ttu-id="ce9fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce9fc-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce9fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce9fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce9fc-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce9fc-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="ce9fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce9fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce9fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce9fc-114">Not supported.</span></span>|
|<span data-ttu-id="ce9fc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce9fc-115">Application</span></span>|<span data-ttu-id="ce9fc-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce9fc-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce9fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce9fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```

## <a name="request-headers"></a><span data-ttu-id="ce9fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce9fc-118">Request headers</span></span>

|<span data-ttu-id="ce9fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ce9fc-119">Name</span></span>|<span data-ttu-id="ce9fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ce9fc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce9fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce9fc-121">Authorization</span></span>|<span data-ttu-id="ce9fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce9fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce9fc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce9fc-124">Request body</span></span>

<span data-ttu-id="ce9fc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce9fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce9fc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9fc-126">Response</span></span>

<span data-ttu-id="ce9fc-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce9fc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ce9fc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce9fc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce9fc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce9fc-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ce9fc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce9fc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reupload_deviceimages_from_virtualendpoint"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}/reupload
```
# <a name="c"></a>[<span data-ttu-id="ce9fc-131">C#</span><span class="sxs-lookup"><span data-stu-id="ce9fc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reupload-deviceimages-from-virtualendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce9fc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce9fc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reupload-deviceimages-from-virtualendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce9fc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce9fc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reupload-deviceimages-from-virtualendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce9fc-134">Java</span><span class="sxs-lookup"><span data-stu-id="ce9fc-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reupload-deviceimages-from-virtualendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce9fc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce9fc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
