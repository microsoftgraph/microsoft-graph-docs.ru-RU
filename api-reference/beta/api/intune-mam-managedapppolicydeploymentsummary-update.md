---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 480f2f8621e8d85b808ee2dd08306c53483fca6b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157955"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="2d700-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2d700-103">Update managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="2d700-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d700-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d700-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d700-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d700-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d700-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d700-107">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d700-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d700-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2d700-108">Prerequisites</span></span>
<span data-ttu-id="2d700-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d700-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d700-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d700-111">Permission type</span></span>|<span data-ttu-id="2d700-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d700-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d700-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d700-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d700-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d700-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d700-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d700-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d700-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d700-116">Not supported.</span></span>|
|<span data-ttu-id="2d700-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d700-117">Application</span></span>|<span data-ttu-id="2d700-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d700-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d700-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d700-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2d700-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2d700-120">Request headers</span></span>
|<span data-ttu-id="2d700-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d700-121">Header</span></span>|<span data-ttu-id="2d700-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2d700-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d700-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d700-123">Authorization</span></span>|<span data-ttu-id="2d700-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d700-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d700-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2d700-125">Accept</span></span>|<span data-ttu-id="2d700-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d700-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d700-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d700-127">Request body</span></span>
<span data-ttu-id="2d700-128">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d700-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="2d700-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d700-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="2d700-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d700-130">Property</span></span>|<span data-ttu-id="2d700-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d700-131">Type</span></span>|<span data-ttu-id="2d700-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d700-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d700-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2d700-133">displayName</span></span>|<span data-ttu-id="2d700-134">String</span><span class="sxs-lookup"><span data-stu-id="2d700-134">String</span></span>|<span data-ttu-id="2d700-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d700-135">Not yet documented</span></span>|
|<span data-ttu-id="2d700-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="2d700-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="2d700-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2d700-137">Int32</span></span>|<span data-ttu-id="2d700-138">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d700-138">Not yet documented</span></span>|
|<span data-ttu-id="2d700-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="2d700-139">lastRefreshTime</span></span>|<span data-ttu-id="2d700-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d700-140">DateTimeOffset</span></span>|<span data-ttu-id="2d700-141">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d700-141">Not yet documented</span></span>|
|<span data-ttu-id="2d700-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="2d700-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="2d700-143">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d700-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="2d700-144">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2d700-144">Not yet documented</span></span>|
|<span data-ttu-id="2d700-145">id</span><span class="sxs-lookup"><span data-stu-id="2d700-145">id</span></span>|<span data-ttu-id="2d700-146">String</span><span class="sxs-lookup"><span data-stu-id="2d700-146">String</span></span>|<span data-ttu-id="2d700-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d700-147">Key of the entity.</span></span>|
|<span data-ttu-id="2d700-148">version</span><span class="sxs-lookup"><span data-stu-id="2d700-148">version</span></span>|<span data-ttu-id="2d700-149">String</span><span class="sxs-lookup"><span data-stu-id="2d700-149">String</span></span>|<span data-ttu-id="2d700-150">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="2d700-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2d700-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d700-151">Response</span></span>
<span data-ttu-id="2d700-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d700-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d700-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2d700-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d700-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d700-154">Request</span></span>
<span data-ttu-id="2d700-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d700-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 589

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="2d700-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d700-156">Response</span></span>
<span data-ttu-id="2d700-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d700-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 638

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.windowsAppIdentifier",
        "windowsAppId": "Windows App Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```




