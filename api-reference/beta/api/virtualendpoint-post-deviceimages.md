---
title: Создание Клаудпкдевицеимаже
description: Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 4cbfb96f6adf70a197b3d648d1bddb4cd405a1c9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563473"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="6c677-103">Создание Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="6c677-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="6c677-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c677-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c677-105">Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="6c677-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="6c677-106">Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="6c677-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="6c677-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c677-107">Permissions</span></span>

<span data-ttu-id="6c677-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c677-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c677-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c677-110">Permission type</span></span>|<span data-ttu-id="6c677-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c677-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c677-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c677-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c677-113">Клаудпк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6c677-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="6c677-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c677-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c677-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c677-115">Not supported.</span></span>|
|<span data-ttu-id="6c677-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c677-116">Application</span></span>|<span data-ttu-id="6c677-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c677-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c677-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c677-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="6c677-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c677-119">Request headers</span></span>

| <span data-ttu-id="6c677-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6c677-120">Name</span></span>          | <span data-ttu-id="6c677-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6c677-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="6c677-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c677-122">Authorization</span></span> | <span data-ttu-id="6c677-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c677-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c677-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c677-125">Content-Type</span></span>  | <span data-ttu-id="6c677-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c677-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c677-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c677-128">Request body</span></span>

<span data-ttu-id="6c677-129">В тексте запроса добавьте представление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c677-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="6c677-130">В следующей таблице приведены свойства, необходимые при создании [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="6c677-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="6c677-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c677-131">Property</span></span>|<span data-ttu-id="6c677-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6c677-132">Type</span></span>|<span data-ttu-id="6c677-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6c677-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c677-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6c677-134">displayName</span></span>|<span data-ttu-id="6c677-135">String</span><span class="sxs-lookup"><span data-stu-id="6c677-135">String</span></span>|<span data-ttu-id="6c677-136">Отображаемое имя изображения.</span><span class="sxs-lookup"><span data-stu-id="6c677-136">The image's display name.</span></span>|
|<span data-ttu-id="6c677-137">саурцеимажересаурцеид</span><span class="sxs-lookup"><span data-stu-id="6c677-137">sourceImageResourceId</span></span>|<span data-ttu-id="6c677-138">String</span><span class="sxs-lookup"><span data-stu-id="6c677-138">String</span></span>|<span data-ttu-id="6c677-139">Идентификатор исходного ресурса изображения в Azure.</span><span class="sxs-lookup"><span data-stu-id="6c677-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="6c677-140">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.компуте/имажес/{имаженаме}".</span><span class="sxs-lookup"><span data-stu-id="6c677-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="6c677-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6c677-141">operatingSystem</span></span>|<span data-ttu-id="6c677-142">String</span><span class="sxs-lookup"><span data-stu-id="6c677-142">String</span></span>|<span data-ttu-id="6c677-143">Операционная система изображения.</span><span class="sxs-lookup"><span data-stu-id="6c677-143">The image's operating system.</span></span> <span data-ttu-id="6c677-144">Пример: Windows 10 Корпоративная.</span><span class="sxs-lookup"><span data-stu-id="6c677-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="6c677-145">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="6c677-145">osBuildNumber</span></span>|<span data-ttu-id="6c677-146">String</span><span class="sxs-lookup"><span data-stu-id="6c677-146">String</span></span>|<span data-ttu-id="6c677-147">Версия сборки ОС образа.</span><span class="sxs-lookup"><span data-stu-id="6c677-147">The image's OS build version.</span></span> <span data-ttu-id="6c677-148">Пример: 1909.</span><span class="sxs-lookup"><span data-stu-id="6c677-148">For example: 1909.</span></span>|
|<span data-ttu-id="6c677-149">version</span><span class="sxs-lookup"><span data-stu-id="6c677-149">version</span></span>|<span data-ttu-id="6c677-150">String</span><span class="sxs-lookup"><span data-stu-id="6c677-150">String</span></span>|<span data-ttu-id="6c677-151">Версия изображения.</span><span class="sxs-lookup"><span data-stu-id="6c677-151">The image version.</span></span> <span data-ttu-id="6c677-152">Например: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="6c677-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="6c677-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c677-153">Response</span></span>

<span data-ttu-id="6c677-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c677-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c677-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c677-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c677-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c677-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c677-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c677-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6c677-158">C#</span><span class="sxs-lookup"><span data-stu-id="6c677-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcdeviceimage-from-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c677-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c677-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcdeviceimage-from-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c677-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c677-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcdeviceimage-from-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c677-161">Java</span><span class="sxs-lookup"><span data-stu-id="6c677-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcdeviceimage-from-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c677-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c677-162">Response</span></span>

<span data-ttu-id="6c677-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6c677-163">**Note:** The response object shown here might be shortened for readability.</span></span>
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
