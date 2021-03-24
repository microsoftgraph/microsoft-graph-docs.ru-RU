---
title: Создание windowsFeatureUpdateCatalogItem
description: Создайте новый объект windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af504a01a4a32e739bdc2faff823fc6192d5c8bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134363"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="375e5-103">Создание windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="375e5-103">Create windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="375e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="375e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="375e5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="375e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="375e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="375e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="375e5-107">Создайте [новый объект windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="375e5-107">Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="375e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="375e5-108">Prerequisites</span></span>
<span data-ttu-id="375e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="375e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="375e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="375e5-111">Permission type</span></span>|<span data-ttu-id="375e5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="375e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="375e5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="375e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="375e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="375e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="375e5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="375e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="375e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="375e5-116">Not supported.</span></span>|
|<span data-ttu-id="375e5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="375e5-117">Application</span></span>|<span data-ttu-id="375e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="375e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="375e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="375e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="375e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="375e5-120">Request headers</span></span>
|<span data-ttu-id="375e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="375e5-121">Header</span></span>|<span data-ttu-id="375e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="375e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="375e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="375e5-123">Authorization</span></span>|<span data-ttu-id="375e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="375e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="375e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="375e5-125">Accept</span></span>|<span data-ttu-id="375e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="375e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="375e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="375e5-127">Request body</span></span>
<span data-ttu-id="375e5-128">В теле запроса поставляем представление JSON для объекта windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="375e5-128">In the request body, supply a JSON representation for the windowsFeatureUpdateCatalogItem object.</span></span>

<span data-ttu-id="375e5-129">В следующей таблице показаны свойства, необходимые при создании windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="375e5-129">The following table shows the properties that are required when you create the windowsFeatureUpdateCatalogItem.</span></span>

|<span data-ttu-id="375e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="375e5-130">Property</span></span>|<span data-ttu-id="375e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="375e5-131">Type</span></span>|<span data-ttu-id="375e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="375e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="375e5-133">id</span><span class="sxs-lookup"><span data-stu-id="375e5-133">id</span></span>|<span data-ttu-id="375e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="375e5-134">String</span></span>|<span data-ttu-id="375e5-135">ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="375e5-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="375e5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="375e5-136">displayName</span></span>|<span data-ttu-id="375e5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="375e5-137">String</span></span>|<span data-ttu-id="375e5-138">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="375e5-138">The display name for the catalog item.</span></span> <span data-ttu-id="375e5-139">Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="375e5-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="375e5-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="375e5-140">releaseDateTime</span></span>|<span data-ttu-id="375e5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="375e5-141">DateTimeOffset</span></span>|<span data-ttu-id="375e5-142">Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="375e5-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="375e5-143">version</span><span class="sxs-lookup"><span data-stu-id="375e5-143">version</span></span>|<span data-ttu-id="375e5-144">String</span><span class="sxs-lookup"><span data-stu-id="375e5-144">String</span></span>|<span data-ttu-id="375e5-145">Версия обновления функций</span><span class="sxs-lookup"><span data-stu-id="375e5-145">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="375e5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="375e5-146">Response</span></span>
<span data-ttu-id="375e5-147">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="375e5-147">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="375e5-148">Пример</span><span class="sxs-lookup"><span data-stu-id="375e5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="375e5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="375e5-149">Request</span></span>
<span data-ttu-id="375e5-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="375e5-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="375e5-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="375e5-151">Response</span></span>
<span data-ttu-id="375e5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="375e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




