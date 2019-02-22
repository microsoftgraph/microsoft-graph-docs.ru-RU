---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a46793ace5d6574740633fdd204bd4d11865ca9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165543"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="c3a6f-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="c3a6f-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="c3a6f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a6f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a6f-106">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c3a6f-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a6f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c3a6f-107">Prerequisites</span></span>
<span data-ttu-id="c3a6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c3a6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3a6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3a6f-110">Permission type</span></span>|<span data-ttu-id="c3a6f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3a6f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3a6f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3a6f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a6f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3a6f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-115">Not supported.</span></span>|
|<span data-ttu-id="c3a6f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3a6f-116">Application</span></span>|<span data-ttu-id="c3a6f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a6f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3a6f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c3a6f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3a6f-119">Request headers</span></span>
|<span data-ttu-id="c3a6f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3a6f-120">Header</span></span>|<span data-ttu-id="c3a6f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c3a6f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a6f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3a6f-122">Authorization</span></span>|<span data-ttu-id="c3a6f-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c3a6f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a6f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c3a6f-124">Accept</span></span>|<span data-ttu-id="c3a6f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a6f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a6f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3a6f-126">Request body</span></span>
<span data-ttu-id="c3a6f-127">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="c3a6f-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c3a6f-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="c3a6f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3a6f-129">Property</span></span>|<span data-ttu-id="c3a6f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c3a6f-130">Type</span></span>|<span data-ttu-id="c3a6f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a6f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a6f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c3a6f-132">displayName</span></span>|<span data-ttu-id="c3a6f-133">String</span><span class="sxs-lookup"><span data-stu-id="c3a6f-133">String</span></span>|<span data-ttu-id="c3a6f-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3a6f-134">Not yet documented</span></span>|
|<span data-ttu-id="c3a6f-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="c3a6f-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="c3a6f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c3a6f-136">Int32</span></span>|<span data-ttu-id="c3a6f-137">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="c3a6f-137">Not yet documented</span></span>|
|<span data-ttu-id="c3a6f-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="c3a6f-138">lastRefreshTime</span></span>|<span data-ttu-id="c3a6f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a6f-139">DateTimeOffset</span></span>|<span data-ttu-id="c3a6f-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3a6f-140">Not yet documented</span></span>|
|<span data-ttu-id="c3a6f-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="c3a6f-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="c3a6f-142">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a6f-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="c3a6f-143">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3a6f-143">Not yet documented</span></span>|
|<span data-ttu-id="c3a6f-144">id</span><span class="sxs-lookup"><span data-stu-id="c3a6f-144">id</span></span>|<span data-ttu-id="c3a6f-145">String</span><span class="sxs-lookup"><span data-stu-id="c3a6f-145">String</span></span>|<span data-ttu-id="c3a6f-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-146">Key of the entity.</span></span>|
|<span data-ttu-id="c3a6f-147">version</span><span class="sxs-lookup"><span data-stu-id="c3a6f-147">version</span></span>|<span data-ttu-id="c3a6f-148">String</span><span class="sxs-lookup"><span data-stu-id="c3a6f-148">String</span></span>|<span data-ttu-id="c3a6f-149">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c3a6f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3a6f-150">Response</span></span>
<span data-ttu-id="c3a6f-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a6f-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a6f-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a6f-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a6f-153">Request</span></span>
<span data-ttu-id="c3a6f-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3a6f-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3a6f-155">Response</span></span>
<span data-ttu-id="c3a6f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3a6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




