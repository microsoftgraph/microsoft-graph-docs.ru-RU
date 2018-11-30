---
title: Обновление объекта managedAppPolicyDeploymentSummary
description: Обновление свойств объекта managedAppPolicyDeploymentSummary.
ms.openlocfilehash: 2c0bf77e3dbd3720bcb0cfea28d69155174fb776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082809"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="cb229-103">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cb229-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="cb229-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb229-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb229-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb229-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb229-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb229-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb229-107">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cb229-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb229-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb229-108">Prerequisites</span></span>
<span data-ttu-id="cb229-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb229-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb229-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb229-111">Permission type</span></span>|<span data-ttu-id="cb229-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb229-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb229-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb229-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb229-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb229-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb229-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb229-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb229-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb229-116">Not supported.</span></span>|
|<span data-ttu-id="cb229-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb229-117">Application</span></span>|<span data-ttu-id="cb229-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb229-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb229-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb229-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cb229-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb229-120">Request headers</span></span>
|<span data-ttu-id="cb229-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb229-121">Header</span></span>|<span data-ttu-id="cb229-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb229-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb229-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb229-123">Authorization</span></span>|<span data-ttu-id="cb229-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb229-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb229-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb229-125">Accept</span></span>|<span data-ttu-id="cb229-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb229-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb229-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb229-127">Request body</span></span>
<span data-ttu-id="cb229-128">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb229-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="cb229-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cb229-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="cb229-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb229-130">Property</span></span>|<span data-ttu-id="cb229-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb229-131">Type</span></span>|<span data-ttu-id="cb229-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb229-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb229-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cb229-133">displayName</span></span>|<span data-ttu-id="cb229-134">String</span><span class="sxs-lookup"><span data-stu-id="cb229-134">String</span></span>|<span data-ttu-id="cb229-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb229-135">Not yet documented</span></span>|
|<span data-ttu-id="cb229-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="cb229-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="cb229-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cb229-137">Int32</span></span>|<span data-ttu-id="cb229-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb229-138">Not yet documented</span></span>|
|<span data-ttu-id="cb229-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="cb229-139">lastRefreshTime</span></span>|<span data-ttu-id="cb229-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb229-140">DateTimeOffset</span></span>|<span data-ttu-id="cb229-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb229-141">Not yet documented</span></span>|
|<span data-ttu-id="cb229-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="cb229-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="cb229-143">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb229-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="cb229-144">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb229-144">Not yet documented</span></span>|
|<span data-ttu-id="cb229-145">id</span><span class="sxs-lookup"><span data-stu-id="cb229-145">id</span></span>|<span data-ttu-id="cb229-146">String</span><span class="sxs-lookup"><span data-stu-id="cb229-146">String</span></span>|<span data-ttu-id="cb229-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb229-147">Key of the entity.</span></span>|
|<span data-ttu-id="cb229-148">version</span><span class="sxs-lookup"><span data-stu-id="cb229-148">version</span></span>|<span data-ttu-id="cb229-149">String</span><span class="sxs-lookup"><span data-stu-id="cb229-149">String</span></span>|<span data-ttu-id="cb229-150">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="cb229-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="cb229-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb229-151">Response</span></span>
<span data-ttu-id="cb229-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb229-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb229-153">Пример</span><span class="sxs-lookup"><span data-stu-id="cb229-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb229-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb229-154">Request</span></span>
<span data-ttu-id="cb229-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb229-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
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

### <a name="response"></a><span data-ttu-id="cb229-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb229-156">Response</span></span>
<span data-ttu-id="cb229-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb229-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





