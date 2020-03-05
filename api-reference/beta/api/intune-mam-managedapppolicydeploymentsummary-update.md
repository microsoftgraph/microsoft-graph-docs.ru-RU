---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b95c208cef65d23418ce06c97d8a0a68eb755a06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463505"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="84ffb-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="84ffb-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="84ffb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84ffb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ffb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84ffb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ffb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84ffb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ffb-107">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="84ffb-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ffb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="84ffb-108">Prerequisites</span></span>
<span data-ttu-id="84ffb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84ffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84ffb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84ffb-111">Permission type</span></span>|<span data-ttu-id="84ffb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84ffb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ffb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84ffb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84ffb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ffb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84ffb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84ffb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ffb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84ffb-116">Not supported.</span></span>|
|<span data-ttu-id="84ffb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84ffb-117">Application</span></span>|<span data-ttu-id="84ffb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ffb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ffb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84ffb-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="84ffb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="84ffb-120">Request headers</span></span>
|<span data-ttu-id="84ffb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84ffb-121">Header</span></span>|<span data-ttu-id="84ffb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84ffb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ffb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84ffb-123">Authorization</span></span>|<span data-ttu-id="84ffb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84ffb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ffb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84ffb-125">Accept</span></span>|<span data-ttu-id="84ffb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84ffb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ffb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84ffb-127">Request body</span></span>
<span data-ttu-id="84ffb-128">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84ffb-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="84ffb-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="84ffb-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="84ffb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84ffb-130">Property</span></span>|<span data-ttu-id="84ffb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84ffb-131">Type</span></span>|<span data-ttu-id="84ffb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84ffb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ffb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="84ffb-133">displayName</span></span>|<span data-ttu-id="84ffb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="84ffb-134">String</span></span>|<span data-ttu-id="84ffb-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84ffb-135">Not yet documented</span></span>|
|<span data-ttu-id="84ffb-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="84ffb-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="84ffb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="84ffb-137">Int32</span></span>|<span data-ttu-id="84ffb-138">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="84ffb-138">Not yet documented</span></span>|
|<span data-ttu-id="84ffb-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="84ffb-139">lastRefreshTime</span></span>|<span data-ttu-id="84ffb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84ffb-140">DateTimeOffset</span></span>|<span data-ttu-id="84ffb-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84ffb-141">Not yet documented</span></span>|
|<span data-ttu-id="84ffb-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="84ffb-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="84ffb-143">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="84ffb-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="84ffb-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="84ffb-144">Not yet documented</span></span>|
|<span data-ttu-id="84ffb-145">id</span><span class="sxs-lookup"><span data-stu-id="84ffb-145">id</span></span>|<span data-ttu-id="84ffb-146">String</span><span class="sxs-lookup"><span data-stu-id="84ffb-146">String</span></span>|<span data-ttu-id="84ffb-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84ffb-147">Key of the entity.</span></span>|
|<span data-ttu-id="84ffb-148">version</span><span class="sxs-lookup"><span data-stu-id="84ffb-148">version</span></span>|<span data-ttu-id="84ffb-149">String</span><span class="sxs-lookup"><span data-stu-id="84ffb-149">String</span></span>|<span data-ttu-id="84ffb-150">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="84ffb-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="84ffb-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="84ffb-151">Response</span></span>
<span data-ttu-id="84ffb-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="84ffb-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ffb-153">Пример</span><span class="sxs-lookup"><span data-stu-id="84ffb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="84ffb-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="84ffb-154">Request</span></span>
<span data-ttu-id="84ffb-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84ffb-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="84ffb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="84ffb-156">Response</span></span>
<span data-ttu-id="84ffb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84ffb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





