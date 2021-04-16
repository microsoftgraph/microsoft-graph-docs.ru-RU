---
title: Создание windowsFeatureUpdateCatalogItem
description: Создайте новый объект windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b7cf68452f5b1c2a0b6d8b4df3a06554e4faae7
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866939"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="1634d-103">Создание windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="1634d-103">Create windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="1634d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1634d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1634d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1634d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1634d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1634d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1634d-107">Создайте [новый объект windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1634d-107">Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1634d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1634d-108">Prerequisites</span></span>
<span data-ttu-id="1634d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1634d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1634d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1634d-111">Permission type</span></span>|<span data-ttu-id="1634d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1634d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1634d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1634d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1634d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1634d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1634d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1634d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1634d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1634d-116">Not supported.</span></span>|
|<span data-ttu-id="1634d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1634d-117">Application</span></span>|<span data-ttu-id="1634d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1634d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1634d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1634d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="1634d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1634d-120">Request headers</span></span>
|<span data-ttu-id="1634d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1634d-121">Header</span></span>|<span data-ttu-id="1634d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1634d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1634d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1634d-123">Authorization</span></span>|<span data-ttu-id="1634d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1634d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1634d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1634d-125">Accept</span></span>|<span data-ttu-id="1634d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1634d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1634d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1634d-127">Request body</span></span>
<span data-ttu-id="1634d-128">В теле запроса поставляем представление JSON для объекта windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="1634d-128">In the request body, supply a JSON representation for the windowsFeatureUpdateCatalogItem object.</span></span>

<span data-ttu-id="1634d-129">В следующей таблице показаны свойства, необходимые при создании windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="1634d-129">The following table shows the properties that are required when you create the windowsFeatureUpdateCatalogItem.</span></span>

|<span data-ttu-id="1634d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1634d-130">Property</span></span>|<span data-ttu-id="1634d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1634d-131">Type</span></span>|<span data-ttu-id="1634d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1634d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1634d-133">id</span><span class="sxs-lookup"><span data-stu-id="1634d-133">id</span></span>|<span data-ttu-id="1634d-134">String</span><span class="sxs-lookup"><span data-stu-id="1634d-134">String</span></span>|<span data-ttu-id="1634d-135">ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1634d-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="1634d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1634d-136">displayName</span></span>|<span data-ttu-id="1634d-137">String</span><span class="sxs-lookup"><span data-stu-id="1634d-137">String</span></span>|<span data-ttu-id="1634d-138">Имя отображения элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="1634d-138">The display name for the catalog item.</span></span> <span data-ttu-id="1634d-139">Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1634d-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="1634d-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1634d-140">releaseDateTime</span></span>|<span data-ttu-id="1634d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1634d-141">DateTimeOffset</span></span>|<span data-ttu-id="1634d-142">Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1634d-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="1634d-143">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="1634d-143">endOfSupportDate</span></span>|<span data-ttu-id="1634d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1634d-144">DateTimeOffset</span></span>|<span data-ttu-id="1634d-145">Последняя поддерживаемая дата для элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="1634d-145">The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="1634d-146">version</span><span class="sxs-lookup"><span data-stu-id="1634d-146">version</span></span>|<span data-ttu-id="1634d-147">String</span><span class="sxs-lookup"><span data-stu-id="1634d-147">String</span></span>|<span data-ttu-id="1634d-148">Версия обновления функций</span><span class="sxs-lookup"><span data-stu-id="1634d-148">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="1634d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1634d-149">Response</span></span>
<span data-ttu-id="1634d-150">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1634d-150">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1634d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1634d-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1634d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1634d-152">Request</span></span>
<span data-ttu-id="1634d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1634d-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="1634d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1634d-154">Response</span></span>
<span data-ttu-id="1634d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1634d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 312

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00",
  "version": "Version value"
}
```




