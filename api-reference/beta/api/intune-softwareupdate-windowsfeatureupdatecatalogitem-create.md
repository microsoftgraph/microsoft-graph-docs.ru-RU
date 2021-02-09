---
title: Создание windowsFeatureUpdateCatalogItem
description: Создание объекта windowsFeatureUpdateCatalogItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc6e1a2d9e6b5f30e00e1212e8513f1af2dec7e0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162408"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="80560-103">Создание windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="80560-103">Create windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="80560-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80560-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80560-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80560-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80560-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80560-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80560-107">Создание объекта [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="80560-107">Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80560-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="80560-108">Prerequisites</span></span>
<span data-ttu-id="80560-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80560-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80560-111">Permission type</span></span>|<span data-ttu-id="80560-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80560-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80560-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80560-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80560-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80560-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80560-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80560-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80560-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80560-116">Not supported.</span></span>|
|<span data-ttu-id="80560-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80560-117">Application</span></span>|<span data-ttu-id="80560-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80560-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80560-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80560-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="80560-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80560-120">Request headers</span></span>
|<span data-ttu-id="80560-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80560-121">Header</span></span>|<span data-ttu-id="80560-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80560-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80560-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80560-123">Authorization</span></span>|<span data-ttu-id="80560-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80560-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80560-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80560-125">Accept</span></span>|<span data-ttu-id="80560-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80560-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80560-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80560-127">Request body</span></span>
<span data-ttu-id="80560-128">В теле запроса укатите представление объекта windowsFeatureUpdateCatalogItem в JSON.</span><span class="sxs-lookup"><span data-stu-id="80560-128">In the request body, supply a JSON representation for the windowsFeatureUpdateCatalogItem object.</span></span>

<span data-ttu-id="80560-129">В следующей таблице показаны свойства, необходимые при создании объекта windowsFeatureUpdateCatalogItem.</span><span class="sxs-lookup"><span data-stu-id="80560-129">The following table shows the properties that are required when you create the windowsFeatureUpdateCatalogItem.</span></span>

|<span data-ttu-id="80560-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="80560-130">Property</span></span>|<span data-ttu-id="80560-131">Тип</span><span class="sxs-lookup"><span data-stu-id="80560-131">Type</span></span>|<span data-ttu-id="80560-132">Описание</span><span class="sxs-lookup"><span data-stu-id="80560-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80560-133">id</span><span class="sxs-lookup"><span data-stu-id="80560-133">id</span></span>|<span data-ttu-id="80560-134">String</span><span class="sxs-lookup"><span data-stu-id="80560-134">String</span></span>|<span data-ttu-id="80560-135">ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="80560-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="80560-136">displayName</span><span class="sxs-lookup"><span data-stu-id="80560-136">displayName</span></span>|<span data-ttu-id="80560-137">String</span><span class="sxs-lookup"><span data-stu-id="80560-137">String</span></span>|<span data-ttu-id="80560-138">Отображаемого имени элемента каталога.</span><span class="sxs-lookup"><span data-stu-id="80560-138">The display name for the catalog item.</span></span> <span data-ttu-id="80560-139">Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="80560-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="80560-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="80560-140">releaseDateTime</span></span>|<span data-ttu-id="80560-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80560-141">DateTimeOffset</span></span>|<span data-ttu-id="80560-142">Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="80560-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="80560-143">version</span><span class="sxs-lookup"><span data-stu-id="80560-143">version</span></span>|<span data-ttu-id="80560-144">String</span><span class="sxs-lookup"><span data-stu-id="80560-144">String</span></span>|<span data-ttu-id="80560-145">Версия обновления функций</span><span class="sxs-lookup"><span data-stu-id="80560-145">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="80560-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="80560-146">Response</span></span>
<span data-ttu-id="80560-147">В случае успеха этот метод возвращает код отклика и объект `201 Created` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="80560-147">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80560-148">Пример</span><span class="sxs-lookup"><span data-stu-id="80560-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="80560-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="80560-149">Request</span></span>
<span data-ttu-id="80560-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80560-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80560-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="80560-151">Response</span></span>
<span data-ttu-id="80560-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80560-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




