---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
author: tfitzmac
ms.openlocfilehash: e123c07722e9bd4baf2cab7bfd5f53516b37a949
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342961"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="11438-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="11438-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="11438-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11438-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11438-105">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11438-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11438-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11438-106">Prerequisites</span></span>
<span data-ttu-id="11438-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11438-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11438-109">Permission type</span></span>|<span data-ttu-id="11438-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11438-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11438-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11438-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11438-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11438-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11438-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11438-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11438-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11438-114">Not supported.</span></span>|
|<span data-ttu-id="11438-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11438-115">Application</span></span>|<span data-ttu-id="11438-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11438-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11438-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11438-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="11438-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11438-118">Request headers</span></span>
|<span data-ttu-id="11438-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11438-119">Header</span></span>|<span data-ttu-id="11438-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11438-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11438-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11438-121">Authorization</span></span>|<span data-ttu-id="11438-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="11438-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11438-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11438-123">Accept</span></span>|<span data-ttu-id="11438-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11438-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11438-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11438-125">Request body</span></span>
<span data-ttu-id="11438-126">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11438-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="11438-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="11438-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="11438-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="11438-128">Property</span></span>|<span data-ttu-id="11438-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11438-129">Type</span></span>|<span data-ttu-id="11438-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11438-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11438-131">displayName</span><span class="sxs-lookup"><span data-stu-id="11438-131">displayName</span></span>|<span data-ttu-id="11438-132">Строка</span><span class="sxs-lookup"><span data-stu-id="11438-132">String</span></span>|<span data-ttu-id="11438-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11438-133">Not yet documented</span></span>|
|<span data-ttu-id="11438-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="11438-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="11438-135">Int32</span><span class="sxs-lookup"><span data-stu-id="11438-135">Int32</span></span>|<span data-ttu-id="11438-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11438-136">Not yet documented</span></span>|
|<span data-ttu-id="11438-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="11438-137">lastRefreshTime</span></span>|<span data-ttu-id="11438-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11438-138">DateTimeOffset</span></span>|<span data-ttu-id="11438-139">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11438-139">Not yet documented</span></span>|
|<span data-ttu-id="11438-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="11438-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="11438-141">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="11438-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="11438-142">Н/Д</span><span class="sxs-lookup"><span data-stu-id="11438-142">Not yet documented</span></span>|
|<span data-ttu-id="11438-143">id</span><span class="sxs-lookup"><span data-stu-id="11438-143">id</span></span>|<span data-ttu-id="11438-144">Строка</span><span class="sxs-lookup"><span data-stu-id="11438-144">String</span></span>|<span data-ttu-id="11438-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11438-145">Key of the entity.</span></span>|
|<span data-ttu-id="11438-146">version</span><span class="sxs-lookup"><span data-stu-id="11438-146">version</span></span>|<span data-ttu-id="11438-147">Строка</span><span class="sxs-lookup"><span data-stu-id="11438-147">String</span></span>|<span data-ttu-id="11438-148">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="11438-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="11438-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="11438-149">Response</span></span>
<span data-ttu-id="11438-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11438-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11438-151">Пример</span><span class="sxs-lookup"><span data-stu-id="11438-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="11438-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="11438-152">Request</span></span>
<span data-ttu-id="11438-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11438-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11438-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="11438-154">Response</span></span>
<span data-ttu-id="11438-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="11438-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



