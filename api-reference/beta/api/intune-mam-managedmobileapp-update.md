---
title: Обновление объекта managedMobileApp
description: Обновление свойств объекта managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75903750c592b5c6f56316e1e6d18a728dde3750
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064985"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="b7ed4-103">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b7ed4-103">Update managedMobileApp</span></span>

<span data-ttu-id="b7ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7ed4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7ed4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7ed4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7ed4-107">Обновление свойств объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7ed4-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7ed4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7ed4-108">Prerequisites</span></span>
<span data-ttu-id="b7ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7ed4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7ed4-111">Permission type</span></span>|<span data-ttu-id="b7ed4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7ed4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7ed4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7ed4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7ed4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7ed4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7ed4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7ed4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7ed4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-116">Not supported.</span></span>|
|<span data-ttu-id="b7ed4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7ed4-117">Application</span></span>|<span data-ttu-id="b7ed4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7ed4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7ed4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7ed4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b7ed4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b7ed4-120">Request headers</span></span>
|<span data-ttu-id="b7ed4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7ed4-121">Header</span></span>|<span data-ttu-id="b7ed4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b7ed4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7ed4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7ed4-123">Authorization</span></span>|<span data-ttu-id="b7ed4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7ed4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7ed4-125">Accept</span></span>|<span data-ttu-id="b7ed4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7ed4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7ed4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7ed4-127">Request body</span></span>
<span data-ttu-id="b7ed4-128">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="b7ed4-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7ed4-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="b7ed4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7ed4-130">Property</span></span>|<span data-ttu-id="b7ed4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b7ed4-131">Type</span></span>|<span data-ttu-id="b7ed4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b7ed4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7ed4-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7ed4-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="b7ed4-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7ed4-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b7ed4-135">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="b7ed4-136">id</span><span class="sxs-lookup"><span data-stu-id="b7ed4-136">id</span></span>|<span data-ttu-id="b7ed4-137">String</span><span class="sxs-lookup"><span data-stu-id="b7ed4-137">String</span></span>|<span data-ttu-id="b7ed4-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-138">Key of the entity.</span></span>|
|<span data-ttu-id="b7ed4-139">version</span><span class="sxs-lookup"><span data-stu-id="b7ed4-139">version</span></span>|<span data-ttu-id="b7ed4-140">String</span><span class="sxs-lookup"><span data-stu-id="b7ed4-140">String</span></span>|<span data-ttu-id="b7ed4-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b7ed4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ed4-142">Response</span></span>
<span data-ttu-id="b7ed4-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7ed4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="b7ed4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7ed4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ed4-145">Request</span></span>
<span data-ttu-id="b7ed4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b7ed4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ed4-147">Response</span></span>
<span data-ttu-id="b7ed4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7ed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```






