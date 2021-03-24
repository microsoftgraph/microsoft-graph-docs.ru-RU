---
title: Обновление windowsFeatureUpdateCatalogItem
description: Обновите свойства объекта windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 612fa821456eede187bb385c8e2ed091f08d8385
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134300"
---
# <a name="update-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="5db9b-103">Обновление windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="5db9b-103">Update windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="5db9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5db9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5db9b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5db9b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5db9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5db9b-107">Обновите свойства [объекта windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-107">Update the properties of a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5db9b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5db9b-108">Prerequisites</span></span>
<span data-ttu-id="5db9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5db9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db9b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db9b-111">Permission type</span></span>|<span data-ttu-id="5db9b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db9b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5db9b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5db9b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db9b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5db9b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db9b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db9b-116">Not supported.</span></span>|
|<span data-ttu-id="5db9b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5db9b-117">Application</span></span>|<span data-ttu-id="5db9b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db9b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db9b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="5db9b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5db9b-120">Request headers</span></span>
|<span data-ttu-id="5db9b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5db9b-121">Header</span></span>|<span data-ttu-id="5db9b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5db9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5db9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5db9b-123">Authorization</span></span>|<span data-ttu-id="5db9b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5db9b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5db9b-125">Accept</span></span>|<span data-ttu-id="5db9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5db9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5db9b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5db9b-127">Request body</span></span>
<span data-ttu-id="5db9b-128">В теле запроса поставляем представление JSON для [объекта windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="5db9b-129">В следующей таблице показаны свойства, необходимые при создании [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md).</span></span>

|<span data-ttu-id="5db9b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5db9b-130">Property</span></span>|<span data-ttu-id="5db9b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5db9b-131">Type</span></span>|<span data-ttu-id="5db9b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5db9b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5db9b-133">id</span><span class="sxs-lookup"><span data-stu-id="5db9b-133">id</span></span>|<span data-ttu-id="5db9b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5db9b-134">String</span></span>|<span data-ttu-id="5db9b-135">ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="5db9b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5db9b-136">displayName</span></span>|<span data-ttu-id="5db9b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5db9b-137">String</span></span>|<span data-ttu-id="5db9b-138">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="5db9b-138">The display name for the catalog item.</span></span> <span data-ttu-id="5db9b-139">Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="5db9b-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="5db9b-140">releaseDateTime</span></span>|<span data-ttu-id="5db9b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db9b-141">DateTimeOffset</span></span>|<span data-ttu-id="5db9b-142">Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="5db9b-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="5db9b-143">version</span><span class="sxs-lookup"><span data-stu-id="5db9b-143">version</span></span>|<span data-ttu-id="5db9b-144">String</span><span class="sxs-lookup"><span data-stu-id="5db9b-144">String</span></span>|<span data-ttu-id="5db9b-145">Версия обновления функций</span><span class="sxs-lookup"><span data-stu-id="5db9b-145">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="5db9b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db9b-146">Response</span></span>
<span data-ttu-id="5db9b-147">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5db9b-147">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db9b-148">Пример</span><span class="sxs-lookup"><span data-stu-id="5db9b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="5db9b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db9b-149">Request</span></span>
<span data-ttu-id="5db9b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db9b-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5db9b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db9b-151">Response</span></span>
<span data-ttu-id="5db9b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5db9b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```




