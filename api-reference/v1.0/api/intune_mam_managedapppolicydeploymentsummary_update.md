# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="4bf4e-101">Обновление объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="4bf4e-101">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="4bf4e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bf4e-103">Обновление свойств объекта [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4bf4e-103">Update the properties of a [calendar](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bf4e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4bf4e-104">Prerequisites</span></span>
<span data-ttu-id="4bf4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4bf4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bf4e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4bf4e-107">Permission type</span></span>|<span data-ttu-id="4bf4e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4bf4e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bf4e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4bf4e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4bf4e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bf4e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4bf4e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4bf4e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bf4e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-112">Not supported.</span></span>|
|<span data-ttu-id="4bf4e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4bf4e-113">Application</span></span>|<span data-ttu-id="4bf4e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bf4e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4bf4e-115">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4bf4e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4bf4e-116">Request headers</span></span>
|<span data-ttu-id="4bf4e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4bf4e-117">Header</span></span>|<span data-ttu-id="4bf4e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4bf4e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bf4e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bf4e-119">Authorization</span></span>|<span data-ttu-id="4bf4e-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4bf4e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4bf4e-121">Accept</span></span>|<span data-ttu-id="4bf4e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4bf4e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bf4e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4bf4e-123">Request body</span></span>
<span data-ttu-id="4bf4e-124">В теле запроса добавьте представление объекта [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="4bf4e-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4bf4e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4bf4e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bf4e-126">Property</span></span>|<span data-ttu-id="4bf4e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4bf4e-127">Type</span></span>|<span data-ttu-id="4bf4e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4bf4e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bf4e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4bf4e-129">displayName</span></span>|<span data-ttu-id="4bf4e-130">String</span><span class="sxs-lookup"><span data-stu-id="4bf4e-130">String</span></span>|<span data-ttu-id="4bf4e-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-131">Not yet documented</span></span>|
|<span data-ttu-id="4bf4e-132">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="4bf4e-132">configurationDeployedUserCount</span></span>|<span data-ttu-id="4bf4e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="4bf4e-133">Int32</span></span>|<span data-ttu-id="4bf4e-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-134">Not yet documented</span></span>|
|<span data-ttu-id="4bf4e-135">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="4bf4e-135">lastRefreshTime</span></span>|<span data-ttu-id="4bf4e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bf4e-136">DateTimeOffset</span></span>|<span data-ttu-id="4bf4e-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-137">Not yet documented</span></span>|
|<span data-ttu-id="4bf4e-138">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="4bf4e-138">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="4bf4e-139">Коллекция [managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="4bf4e-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="4bf4e-140">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-140">Not yet documented</span></span>|
|<span data-ttu-id="4bf4e-141">id</span><span class="sxs-lookup"><span data-stu-id="4bf4e-141">id</span></span>|<span data-ttu-id="4bf4e-142">String</span><span class="sxs-lookup"><span data-stu-id="4bf4e-142">String</span></span>|<span data-ttu-id="4bf4e-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-143">Key of the setting.</span></span>|
|<span data-ttu-id="4bf4e-144">version</span><span class="sxs-lookup"><span data-stu-id="4bf4e-144">version</span></span>|<span data-ttu-id="4bf4e-145">String</span><span class="sxs-lookup"><span data-stu-id="4bf4e-145">String</span></span>|<span data-ttu-id="4bf4e-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4bf4e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4bf4e-147">Response</span></span>
<span data-ttu-id="4bf4e-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bf4e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4bf4e-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bf4e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4bf4e-150">Request</span></span>
<span data-ttu-id="4bf4e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="4bf4e-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="4bf4e-152">Response</span></span>
<span data-ttu-id="4bf4e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4bf4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



