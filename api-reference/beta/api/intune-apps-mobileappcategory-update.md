---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd2d1ef4dae6119456d8b2a9fc1cdf9c12f239e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977462"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="366ea-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="366ea-103">Update mobileAppCategory</span></span>

<span data-ttu-id="366ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="366ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="366ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="366ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="366ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="366ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="366ea-107">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="366ea-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="366ea-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="366ea-108">Prerequisites</span></span>
<span data-ttu-id="366ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="366ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="366ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="366ea-111">Permission type</span></span>|<span data-ttu-id="366ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="366ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="366ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="366ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="366ea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="366ea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="366ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="366ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="366ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="366ea-116">Not supported.</span></span>|
|<span data-ttu-id="366ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="366ea-117">Application</span></span>|<span data-ttu-id="366ea-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="366ea-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="366ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="366ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="366ea-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="366ea-120">Request headers</span></span>
|<span data-ttu-id="366ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="366ea-121">Header</span></span>|<span data-ttu-id="366ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="366ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="366ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="366ea-123">Authorization</span></span>|<span data-ttu-id="366ea-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="366ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="366ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="366ea-125">Accept</span></span>|<span data-ttu-id="366ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="366ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="366ea-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="366ea-127">Request body</span></span>
<span data-ttu-id="366ea-128">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="366ea-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="366ea-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="366ea-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="366ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="366ea-130">Property</span></span>|<span data-ttu-id="366ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="366ea-131">Type</span></span>|<span data-ttu-id="366ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="366ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="366ea-133">id</span><span class="sxs-lookup"><span data-stu-id="366ea-133">id</span></span>|<span data-ttu-id="366ea-134">String</span><span class="sxs-lookup"><span data-stu-id="366ea-134">String</span></span>|<span data-ttu-id="366ea-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="366ea-135">The key of the entity.</span></span>|
|<span data-ttu-id="366ea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="366ea-136">displayName</span></span>|<span data-ttu-id="366ea-137">String</span><span class="sxs-lookup"><span data-stu-id="366ea-137">String</span></span>|<span data-ttu-id="366ea-138">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="366ea-138">The name of the app category.</span></span>|
|<span data-ttu-id="366ea-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="366ea-139">lastModifiedDateTime</span></span>|<span data-ttu-id="366ea-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="366ea-140">DateTimeOffset</span></span>|<span data-ttu-id="366ea-141">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="366ea-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="366ea-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="366ea-142">Response</span></span>
<span data-ttu-id="366ea-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="366ea-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="366ea-144">Пример</span><span class="sxs-lookup"><span data-stu-id="366ea-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="366ea-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="366ea-145">Request</span></span>
<span data-ttu-id="366ea-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="366ea-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="366ea-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="366ea-147">Response</span></span>
<span data-ttu-id="366ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="366ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






