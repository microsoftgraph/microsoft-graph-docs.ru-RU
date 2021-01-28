---
title: Тип ресурса cloudPcDeviceImage
description: Представляет ресурс изображения на облачном компьютере.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14e3f28d9e7d91df953405bc36afff4d3405c886
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033901"
---
# <a name="cloudpcdeviceimage-resource-type"></a><span data-ttu-id="84f73-103">Тип ресурса cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-103">cloudPcDeviceImage resource type</span></span>

<span data-ttu-id="84f73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84f73-105">Представляет ресурс изображения на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="84f73-105">Represents the image resource on cloud PC.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="84f73-106">Методы</span><span class="sxs-lookup"><span data-stu-id="84f73-106">Methods</span></span>

|<span data-ttu-id="84f73-107">Метод</span><span class="sxs-lookup"><span data-stu-id="84f73-107">Method</span></span>|<span data-ttu-id="84f73-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="84f73-108">Return type</span></span>|<span data-ttu-id="84f73-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84f73-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84f73-110">Список deviceImages</span><span class="sxs-lookup"><span data-stu-id="84f73-110">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="84f73-111">[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-111">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="84f73-112">Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-112">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="84f73-113">Get cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-113">Get cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-get.md)|[<span data-ttu-id="84f73-114">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-114">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="84f73-115">Чтение свойств и связей объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-115">Read the properties and relationships of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="84f73-116">Создание cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-116">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="84f73-117">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-117">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="84f73-118">Создание объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-118">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="84f73-119">Удаление cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="84f73-119">Delete cloudPcDeviceImage</span></span>](../api/cloudpcdeviceimage-delete.md)|<span data-ttu-id="84f73-120">Нет</span><span class="sxs-lookup"><span data-stu-id="84f73-120">None</span></span>|<span data-ttu-id="84f73-121">Удаление объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-121">Delete a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="84f73-122">getSourceImages</span><span class="sxs-lookup"><span data-stu-id="84f73-122">getSourceImages</span></span>](../api/cloudpcdeviceimage-getsourceimages.md)|<span data-ttu-id="84f73-123">[Коллекция cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-123">[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) collection</span></span>|<span data-ttu-id="84f73-124">Получите [объекты cloudPcSourceDeviceImage.](../resources/cloudpcsourcedeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="84f73-124">Get [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="84f73-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="84f73-125">Properties</span></span>

|<span data-ttu-id="84f73-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="84f73-126">Property</span></span>|<span data-ttu-id="84f73-127">Тип</span><span class="sxs-lookup"><span data-stu-id="84f73-127">Type</span></span>|<span data-ttu-id="84f73-128">Описание</span><span class="sxs-lookup"><span data-stu-id="84f73-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f73-129">id</span><span class="sxs-lookup"><span data-stu-id="84f73-129">id</span></span>|<span data-ttu-id="84f73-130">String</span><span class="sxs-lookup"><span data-stu-id="84f73-130">String</span></span>|<span data-ttu-id="84f73-131">Уникальный идентификатор ресурса изображения на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="84f73-131">Unique identifier for the image resource on cloud PC.</span></span> <span data-ttu-id="84f73-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84f73-132">Read-only.</span></span>|
|<span data-ttu-id="84f73-133">sourceImageResourceId</span><span class="sxs-lookup"><span data-stu-id="84f73-133">sourceImageResourceId</span></span>|<span data-ttu-id="84f73-134">String</span><span class="sxs-lookup"><span data-stu-id="84f73-134">String</span></span>|<span data-ttu-id="84f73-135">ИД ресурса исходных изображений в Azure.</span><span class="sxs-lookup"><span data-stu-id="84f73-135">The ID of the source image resource on Azure.</span></span> <span data-ttu-id="84f73-136">Требуемого формата: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span><span class="sxs-lookup"><span data-stu-id="84f73-136">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".</span></span>|
|<span data-ttu-id="84f73-137">displayName</span><span class="sxs-lookup"><span data-stu-id="84f73-137">displayName</span></span>|<span data-ttu-id="84f73-138">String</span><span class="sxs-lookup"><span data-stu-id="84f73-138">String</span></span>|<span data-ttu-id="84f73-139">Отображаемая фамилия изображения.</span><span class="sxs-lookup"><span data-stu-id="84f73-139">The image's display name.</span></span>|
|<span data-ttu-id="84f73-140">version</span><span class="sxs-lookup"><span data-stu-id="84f73-140">version</span></span>|<span data-ttu-id="84f73-141">String</span><span class="sxs-lookup"><span data-stu-id="84f73-141">String</span></span>|<span data-ttu-id="84f73-142">Версия изображения.</span><span class="sxs-lookup"><span data-stu-id="84f73-142">The image version.</span></span> <span data-ttu-id="84f73-143">Например: 0.0.1, 1.5.13.</span><span class="sxs-lookup"><span data-stu-id="84f73-143">For example: 0.0.1, 1.5.13.</span></span>|
|<span data-ttu-id="84f73-144">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="84f73-144">osBuildNumber</span></span>|<span data-ttu-id="84f73-145">String</span><span class="sxs-lookup"><span data-stu-id="84f73-145">String</span></span>|<span data-ttu-id="84f73-146">Версия сборки ОС образа.</span><span class="sxs-lookup"><span data-stu-id="84f73-146">The image's OS build version.</span></span> <span data-ttu-id="84f73-147">Например: 1909.</span><span class="sxs-lookup"><span data-stu-id="84f73-147">For example: 1909.</span></span>|
|<span data-ttu-id="84f73-148">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="84f73-148">operatingSystem</span></span>|<span data-ttu-id="84f73-149">String</span><span class="sxs-lookup"><span data-stu-id="84f73-149">String</span></span>|<span data-ttu-id="84f73-150">Операционная система образа.</span><span class="sxs-lookup"><span data-stu-id="84f73-150">The image's operating system.</span></span> <span data-ttu-id="84f73-151">Например: Windows 10 Корпоративная.</span><span class="sxs-lookup"><span data-stu-id="84f73-151">For example: Windows 10 Enterprise.</span></span>|
|<span data-ttu-id="84f73-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84f73-152">lastModifiedDateTime</span></span>|<span data-ttu-id="84f73-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84f73-153">DateTimeOffset</span></span>|<span data-ttu-id="84f73-154">Данные и время последнего изменения изображения.</span><span class="sxs-lookup"><span data-stu-id="84f73-154">The data and time that the image was last modified.</span></span> <span data-ttu-id="84f73-155">Время отображается в формате ISO 8601 и времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="84f73-155">The time is shown in ISO 8601 format and  Coordinated Universal Time (UTC) time.</span></span> <span data-ttu-id="84f73-156">Например, полночь 1 января 2014 г. в UTC отображается как "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="84f73-156">For example, midnight UTC on Jan 1, 2014 appears as '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="84f73-157">status</span><span class="sxs-lookup"><span data-stu-id="84f73-157">status</span></span>|<span data-ttu-id="84f73-158">cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-158">cloudPcDeviceImageStatus</span></span>|<span data-ttu-id="84f73-159">Состояние изображения на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="84f73-159">The status of the image on cloud PC.</span></span> <span data-ttu-id="84f73-160">Возможные значения: `pending`, `ready`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="84f73-160">Possible values are: `pending`, `ready`, `failed`.</span></span>|
|<span data-ttu-id="84f73-161">statusDetails</span><span class="sxs-lookup"><span data-stu-id="84f73-161">statusDetails</span></span>|<span data-ttu-id="84f73-162">cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="84f73-162">cloudPcDeviceImageStatusDetails</span></span>|<span data-ttu-id="84f73-163">Сведения о состоянии изображения, которые указывают, почему не удалось отправить, если применимо.</span><span class="sxs-lookup"><span data-stu-id="84f73-163">The details of the image's status, which indicates why the upload failed, if applicable.</span></span> <span data-ttu-id="84f73-164">Возможные значения: `internalServerError`, `sourceImageNotFound`.</span><span class="sxs-lookup"><span data-stu-id="84f73-164">Possible values are: `internalServerError`, `sourceImageNotFound`.</span></span>|

### <a name="cloudpcdeviceimagestatus-values"></a><span data-ttu-id="84f73-165">Значения cloudPcDeviceImageStatus</span><span class="sxs-lookup"><span data-stu-id="84f73-165">cloudPcDeviceImageStatus values</span></span>

|<span data-ttu-id="84f73-166">Member</span><span class="sxs-lookup"><span data-stu-id="84f73-166">Member</span></span>|<span data-ttu-id="84f73-167">Описание</span><span class="sxs-lookup"><span data-stu-id="84f73-167">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84f73-168">pending</span><span class="sxs-lookup"><span data-stu-id="84f73-168">pending</span></span>|<span data-ttu-id="84f73-169">Идет отправка изображения.</span><span class="sxs-lookup"><span data-stu-id="84f73-169">The image upload is in progress.</span></span>|
|<span data-ttu-id="84f73-170">ready</span><span class="sxs-lookup"><span data-stu-id="84f73-170">ready</span></span>|<span data-ttu-id="84f73-171">Изображение готово к использованию на облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="84f73-171">The image is ready for use on Cloud PCs.</span></span>|
|<span data-ttu-id="84f73-172">failed</span><span class="sxs-lookup"><span data-stu-id="84f73-172">failed</span></span>|<span data-ttu-id="84f73-173">Не удалось отправить изображение.</span><span class="sxs-lookup"><span data-stu-id="84f73-173">The image couldn’t be uploaded.</span></span> |

### <a name="cloudpcdeviceimagestatusdetails-values"></a><span data-ttu-id="84f73-174">Значения cloudPcDeviceImageStatusDetails</span><span class="sxs-lookup"><span data-stu-id="84f73-174">cloudPcDeviceImageStatusDetails values</span></span>

|<span data-ttu-id="84f73-175">Member</span><span class="sxs-lookup"><span data-stu-id="84f73-175">Member</span></span>|<span data-ttu-id="84f73-176">Описание</span><span class="sxs-lookup"><span data-stu-id="84f73-176">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84f73-177">internalServerError</span><span class="sxs-lookup"><span data-stu-id="84f73-177">internalServerError</span></span>|<span data-ttu-id="84f73-178">При обработке образа произошла внутренняя ошибка сервера.</span><span class="sxs-lookup"><span data-stu-id="84f73-178">There was an internal server error while processing the image.</span></span>|
|<span data-ttu-id="84f73-179">sourceImageNotFound</span><span class="sxs-lookup"><span data-stu-id="84f73-179">sourceImageNotFound</span></span>|<span data-ttu-id="84f73-180">Исходный образ не является допустимым для предоставления к ней ВМ Для Windows.</span><span class="sxs-lookup"><span data-stu-id="84f73-180">The source image is not valid for provisioning a Windows VM with it.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84f73-181">Связи</span><span class="sxs-lookup"><span data-stu-id="84f73-181">Relationships</span></span>

<span data-ttu-id="84f73-182">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84f73-182">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84f73-183">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="84f73-183">JSON representation</span></span>

<span data-ttu-id="84f73-184">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84f73-184">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
