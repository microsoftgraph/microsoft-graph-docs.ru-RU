---
title: Создание cloudPcDeviceImage
description: Загрузите пользовательский образ ОС, который можно позже настроить на облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: aa0d7ba5a15acacf22cce43e4a4989dabb131118
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873950"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="8395f-103">Создание cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="8395f-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="8395f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8395f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8395f-105">Создание объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="8395f-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="8395f-106">Загрузите пользовательский образ ОС, который можно позже настроить на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="8395f-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8395f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8395f-107">Permissions</span></span>

<span data-ttu-id="8395f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8395f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8395f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8395f-110">Permission type</span></span>|<span data-ttu-id="8395f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8395f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8395f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8395f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8395f-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8395f-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8395f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8395f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8395f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8395f-115">Not supported.</span></span>|
|<span data-ttu-id="8395f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8395f-116">Application</span></span>|<span data-ttu-id="8395f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8395f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8395f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8395f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="8395f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8395f-119">Request headers</span></span>

| <span data-ttu-id="8395f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8395f-120">Name</span></span>          | <span data-ttu-id="8395f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8395f-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="8395f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8395f-122">Authorization</span></span> | <span data-ttu-id="8395f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8395f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8395f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8395f-125">Content-Type</span></span>  | <span data-ttu-id="8395f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8395f-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8395f-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="8395f-128">Request body</span></span>

<span data-ttu-id="8395f-129">В теле запроса укажу представление объекта [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="8395f-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="8395f-130">В следующей таблице показаны свойства, необходимые при создании [объекта cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="8395f-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="8395f-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8395f-131">Property</span></span>|<span data-ttu-id="8395f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8395f-132">Type</span></span>|<span data-ttu-id="8395f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8395f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8395f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8395f-134">displayName</span></span>|<span data-ttu-id="8395f-135">String</span><span class="sxs-lookup"><span data-stu-id="8395f-135">String</span></span>|<span data-ttu-id="8395f-136">Отображаемая фамилия изображения.</span><span class="sxs-lookup"><span data-stu-id="8395f-136">The image's display name.</span></span>|
|<span data-ttu-id="8395f-137">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="8395f-137">sourceImageResourceId</span></span>|<span data-ttu-id="8395f-138">String</span><span class="sxs-lookup"><span data-stu-id="8395f-138">String</span></span>|<span data-ttu-id="8395f-139">ИД ресурса исходных изображений в Azure.</span><span class="sxs-lookup"><span data-stu-id="8395f-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="8395f-140">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="8395f-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="8395f-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="8395f-141">operatingSystem</span></span>|<span data-ttu-id="8395f-142">String</span><span class="sxs-lookup"><span data-stu-id="8395f-142">String</span></span>|<span data-ttu-id="8395f-143">Операционная система образа.</span><span class="sxs-lookup"><span data-stu-id="8395f-143">The image's operating system.</span></span> <span data-ttu-id="8395f-144">Например: Windows 10 Корпоративная.</span><span class="sxs-lookup"><span data-stu-id="8395f-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="8395f-145">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="8395f-145">osBuildNumber</span></span>|<span data-ttu-id="8395f-146">String</span><span class="sxs-lookup"><span data-stu-id="8395f-146">String</span></span>|<span data-ttu-id="8395f-147">Версия сборки ОС образа.</span><span class="sxs-lookup"><span data-stu-id="8395f-147">The image's OS build version.</span></span> <span data-ttu-id="8395f-148">Например: 1909.</span><span class="sxs-lookup"><span data-stu-id="8395f-148">For example: 1909.</span></span>|
|<span data-ttu-id="8395f-149">version</span><span class="sxs-lookup"><span data-stu-id="8395f-149">version</span></span>|<span data-ttu-id="8395f-150">String</span><span class="sxs-lookup"><span data-stu-id="8395f-150">String</span></span>|<span data-ttu-id="8395f-151">Версия изображения.</span><span class="sxs-lookup"><span data-stu-id="8395f-151">The image version.</span></span> <span data-ttu-id="8395f-152">Например: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="8395f-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="8395f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8395f-153">Response</span></span>

<span data-ttu-id="8395f-154">В случае успеха этот метод возвращает код отклика и объект `201 Created` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8395f-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8395f-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="8395f-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8395f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="8395f-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8395f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8395f-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8395f-158">C#</span><span class="sxs-lookup"><span data-stu-id="8395f-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8395f-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8395f-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8395f-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8395f-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8395f-161">Java</span><span class="sxs-lookup"><span data-stu-id="8395f-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8395f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8395f-162">Response</span></span>

<span data-ttu-id="8395f-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8395f-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
