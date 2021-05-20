---
title: Создание cloudPcDeviceImage
description: Upload образ оси, который можно позже использовать на облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e7da8717b9dcbf34d40de5bbcb08247d80d04514
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547094"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="b6619-103">Создание cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="b6619-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="b6619-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6619-105">Создайте новый [объект cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="b6619-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="b6619-106">Upload образ оси, который можно позже использовать на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="b6619-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="b6619-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6619-107">Permissions</span></span>

<span data-ttu-id="b6619-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6619-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6619-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6619-110">Permission type</span></span>|<span data-ttu-id="b6619-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6619-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6619-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6619-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6619-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6619-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="b6619-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6619-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6619-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6619-115">Not supported.</span></span>|
|<span data-ttu-id="b6619-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6619-116">Application</span></span>|<span data-ttu-id="b6619-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6619-117">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6619-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6619-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="b6619-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6619-119">Request headers</span></span>

| <span data-ttu-id="b6619-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b6619-120">Name</span></span>          | <span data-ttu-id="b6619-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b6619-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="b6619-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6619-122">Authorization</span></span> | <span data-ttu-id="b6619-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6619-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b6619-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6619-125">Content-Type</span></span>  | <span data-ttu-id="b6619-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6619-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6619-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6619-128">Request body</span></span>

<span data-ttu-id="b6619-129">В теле запроса поставляем представление JSON объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="b6619-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="b6619-130">В следующей таблице показаны свойства, необходимые при создании [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="b6619-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="b6619-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6619-131">Property</span></span>|<span data-ttu-id="b6619-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b6619-132">Type</span></span>|<span data-ttu-id="b6619-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b6619-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6619-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b6619-134">displayName</span></span>|<span data-ttu-id="b6619-135">String</span><span class="sxs-lookup"><span data-stu-id="b6619-135">String</span></span>|<span data-ttu-id="b6619-136">Имя отображения изображения.</span><span class="sxs-lookup"><span data-stu-id="b6619-136">The image's display name.</span></span>|
|<span data-ttu-id="b6619-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="b6619-137">sourceImageResourceId</span></span>|<span data-ttu-id="b6619-138">String</span><span class="sxs-lookup"><span data-stu-id="b6619-138">String</span></span>|<span data-ttu-id="b6619-139">ID источника ресурса изображений в Azure.</span><span class="sxs-lookup"><span data-stu-id="b6619-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="b6619-140">Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="b6619-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="b6619-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b6619-141">operatingSystem</span></span>|<span data-ttu-id="b6619-142">String</span><span class="sxs-lookup"><span data-stu-id="b6619-142">String</span></span>|<span data-ttu-id="b6619-143">Операционная система изображения.</span><span class="sxs-lookup"><span data-stu-id="b6619-143">The image's operating system.</span></span> <span data-ttu-id="b6619-144">Например: Windows 10 Корпоративная.</span><span class="sxs-lookup"><span data-stu-id="b6619-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="b6619-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b6619-145">osBuildNumber</span></span>|<span data-ttu-id="b6619-146">String</span><span class="sxs-lookup"><span data-stu-id="b6619-146">String</span></span>|<span data-ttu-id="b6619-147">Версия сборки ОС изображения.</span><span class="sxs-lookup"><span data-stu-id="b6619-147">The image's OS build version.</span></span> <span data-ttu-id="b6619-148">Например: 1909.</span><span class="sxs-lookup"><span data-stu-id="b6619-148">For example: 1909.</span></span>|
|<span data-ttu-id="b6619-149">version</span><span class="sxs-lookup"><span data-stu-id="b6619-149">version</span></span>|<span data-ttu-id="b6619-150">String</span><span class="sxs-lookup"><span data-stu-id="b6619-150">String</span></span>|<span data-ttu-id="b6619-151">Версия изображения.</span><span class="sxs-lookup"><span data-stu-id="b6619-151">The image version.</span></span> <span data-ttu-id="b6619-152">Например: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="b6619-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="b6619-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6619-153">Response</span></span>

<span data-ttu-id="b6619-154">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b6619-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6619-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="b6619-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b6619-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6619-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b6619-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6619-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcdeviceimage_from_cloudpcdeviceimage"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}
```
# <a name="c"></a>[<span data-ttu-id="b6619-158">C#</span><span class="sxs-lookup"><span data-stu-id="b6619-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6619-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6619-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6619-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6619-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6619-161">Java</span><span class="sxs-lookup"><span data-stu-id="b6619-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6619-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6619-162">Response</span></span>

<span data-ttu-id="b6619-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b6619-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 508

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "eda7ed64-7705-4079-9d08-c2bd883fffff",
  "displayName": "Display Name value",
  "osBuildNumber": "OS Build Number value",
  "operatingSystem": "Operating System value",
  "version": "Version value",
  "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
  "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
  "status": "pending",
  "statusDetails": null
}
```
