---
title: Создание Клаудпкдевицеимаже
description: Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7b2e60355bfe4db8eee014ac2290c83d146eea37
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378587"
---
# <a name="create-cloudpcdeviceimage"></a><span data-ttu-id="57442-103">Создание Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="57442-103">Create cloudPcDeviceImage</span></span>

<span data-ttu-id="57442-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57442-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57442-105">Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="57442-105">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span> <span data-ttu-id="57442-106">Отправьте настраиваемый образ ОС, который вы можете подготовить к работе на облачных компьютерах.</span><span class="sxs-lookup"><span data-stu-id="57442-106">Upload a custom OS image that you can later provision on cloud PCs.</span></span>

## <a name="permissions"></a><span data-ttu-id="57442-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57442-107">Permissions</span></span>

<span data-ttu-id="57442-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57442-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57442-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57442-110">Permission type</span></span>|<span data-ttu-id="57442-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57442-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57442-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57442-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57442-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57442-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="57442-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57442-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57442-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57442-115">Not supported.</span></span>|
|<span data-ttu-id="57442-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57442-116">Application</span></span>|<span data-ttu-id="57442-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57442-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57442-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57442-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/deviceImages
```

## <a name="request-headers"></a><span data-ttu-id="57442-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57442-119">Request headers</span></span>

| <span data-ttu-id="57442-120">Имя</span><span class="sxs-lookup"><span data-stu-id="57442-120">Name</span></span>          | <span data-ttu-id="57442-121">Описание</span><span class="sxs-lookup"><span data-stu-id="57442-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="57442-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57442-122">Authorization</span></span> | <span data-ttu-id="57442-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57442-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="57442-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57442-125">Content-Type</span></span>  | <span data-ttu-id="57442-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57442-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57442-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57442-128">Request body</span></span>

<span data-ttu-id="57442-129">В тексте запроса добавьте представление объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57442-129">In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>

<span data-ttu-id="57442-130">В следующей таблице приведены свойства, необходимые при создании [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md).</span><span class="sxs-lookup"><span data-stu-id="57442-130">The following table shows the properties that are required when you create the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).</span></span>

|<span data-ttu-id="57442-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="57442-131">Property</span></span>|<span data-ttu-id="57442-132">Тип</span><span class="sxs-lookup"><span data-stu-id="57442-132">Type</span></span>|<span data-ttu-id="57442-133">Описание</span><span class="sxs-lookup"><span data-stu-id="57442-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57442-134">displayName</span><span class="sxs-lookup"><span data-stu-id="57442-134">displayName</span></span>|<span data-ttu-id="57442-135">Строка</span><span class="sxs-lookup"><span data-stu-id="57442-135">String</span></span>|<span data-ttu-id="57442-136">Отображаемое имя изображения.</span><span class="sxs-lookup"><span data-stu-id="57442-136">The image's display name.</span></span>|
|<span data-ttu-id="57442-137">саурцеимажересаурцеид</span><span class="sxs-lookup"><span data-stu-id="57442-137">sourceImageResourceId</span></span>|<span data-ttu-id="57442-138">Строка</span><span class="sxs-lookup"><span data-stu-id="57442-138">String</span></span>|<span data-ttu-id="57442-139">Идентификатор исходного ресурса изображения в Azure.</span><span class="sxs-lookup"><span data-stu-id="57442-139">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="57442-140">Требуемый формат: "/Субскриптионс/{субскриптион-ИД}/ресаурцеграупс/{ресаурцеграупнаме}/провидерс/Микрософт.компуте/имажес/{имаженаме}".</span><span class="sxs-lookup"><span data-stu-id="57442-140">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="57442-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="57442-141">operatingSystem</span></span>|<span data-ttu-id="57442-142">String</span><span class="sxs-lookup"><span data-stu-id="57442-142">String</span></span>|<span data-ttu-id="57442-143">Операционная система изображения.</span><span class="sxs-lookup"><span data-stu-id="57442-143">The image's operating system.</span></span> <span data-ttu-id="57442-144">Пример: Windows 10 Корпоративная.</span><span class="sxs-lookup"><span data-stu-id="57442-144">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="57442-145">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="57442-145">osBuildNumber</span></span>|<span data-ttu-id="57442-146">Строка</span><span class="sxs-lookup"><span data-stu-id="57442-146">String</span></span>|<span data-ttu-id="57442-147">Версия сборки ОС образа.</span><span class="sxs-lookup"><span data-stu-id="57442-147">The image's OS build version.</span></span> <span data-ttu-id="57442-148">Пример: 1909.</span><span class="sxs-lookup"><span data-stu-id="57442-148">For example: 1909.</span></span>|
|<span data-ttu-id="57442-149">version</span><span class="sxs-lookup"><span data-stu-id="57442-149">version</span></span>|<span data-ttu-id="57442-150">String</span><span class="sxs-lookup"><span data-stu-id="57442-150">String</span></span>|<span data-ttu-id="57442-151">Версия изображения.</span><span class="sxs-lookup"><span data-stu-id="57442-151">The image version.</span></span> <span data-ttu-id="57442-152">Например: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="57442-152">For example: 0.0.1, 1.5.13.</span></span>|

## <a name="response"></a><span data-ttu-id="57442-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="57442-153">Response</span></span>

<span data-ttu-id="57442-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57442-154">If successful, this method returns a `201 Created` response code and a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57442-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="57442-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57442-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="57442-156">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="57442-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="57442-157">Response</span></span>

<span data-ttu-id="57442-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57442-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
