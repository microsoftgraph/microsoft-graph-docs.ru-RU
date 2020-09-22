---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 532e882e2d47ce4692ac2f91d0d0ad17d1bf0854
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063172"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="ddec5-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="ddec5-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="ddec5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddec5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddec5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddec5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddec5-106">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ddec5-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddec5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddec5-107">Prerequisites</span></span>
<span data-ttu-id="ddec5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddec5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddec5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddec5-110">Permission type</span></span>|<span data-ttu-id="ddec5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddec5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddec5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddec5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddec5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddec5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddec5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddec5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddec5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddec5-115">Not supported.</span></span>|
|<span data-ttu-id="ddec5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddec5-116">Application</span></span>|<span data-ttu-id="ddec5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddec5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddec5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddec5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="ddec5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddec5-119">Request headers</span></span>
|<span data-ttu-id="ddec5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddec5-120">Header</span></span>|<span data-ttu-id="ddec5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ddec5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddec5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddec5-122">Authorization</span></span>|<span data-ttu-id="ddec5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddec5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddec5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ddec5-124">Accept</span></span>|<span data-ttu-id="ddec5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddec5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddec5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddec5-126">Request body</span></span>
<span data-ttu-id="ddec5-127">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddec5-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="ddec5-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ddec5-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="ddec5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddec5-129">Property</span></span>|<span data-ttu-id="ddec5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ddec5-130">Type</span></span>|<span data-ttu-id="ddec5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ddec5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddec5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ddec5-132">displayName</span></span>|<span data-ttu-id="ddec5-133">String</span><span class="sxs-lookup"><span data-stu-id="ddec5-133">String</span></span>|<span data-ttu-id="ddec5-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ddec5-134">Not yet documented</span></span>|
|<span data-ttu-id="ddec5-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="ddec5-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="ddec5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ddec5-136">Int32</span></span>|<span data-ttu-id="ddec5-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ddec5-137">Not yet documented</span></span>|
|<span data-ttu-id="ddec5-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="ddec5-138">lastRefreshTime</span></span>|<span data-ttu-id="ddec5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddec5-139">DateTimeOffset</span></span>|<span data-ttu-id="ddec5-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ddec5-140">Not yet documented</span></span>|
|<span data-ttu-id="ddec5-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ddec5-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="ddec5-142">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="ddec5-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="ddec5-143">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ddec5-143">Not yet documented</span></span>|
|<span data-ttu-id="ddec5-144">id</span><span class="sxs-lookup"><span data-stu-id="ddec5-144">id</span></span>|<span data-ttu-id="ddec5-145">String</span><span class="sxs-lookup"><span data-stu-id="ddec5-145">String</span></span>|<span data-ttu-id="ddec5-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddec5-146">Key of the entity.</span></span>|
|<span data-ttu-id="ddec5-147">version</span><span class="sxs-lookup"><span data-stu-id="ddec5-147">version</span></span>|<span data-ttu-id="ddec5-148">String</span><span class="sxs-lookup"><span data-stu-id="ddec5-148">String</span></span>|<span data-ttu-id="ddec5-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ddec5-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ddec5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddec5-150">Response</span></span>
<span data-ttu-id="ddec5-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddec5-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddec5-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ddec5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddec5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddec5-153">Request</span></span>
<span data-ttu-id="ddec5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddec5-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ddec5-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddec5-155">Response</span></span>
<span data-ttu-id="ddec5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddec5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```









