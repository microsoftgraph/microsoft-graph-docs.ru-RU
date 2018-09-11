# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="71c3f-101">Обновление объекта managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="71c3f-101">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="71c3f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71c3f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71c3f-103">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="71c3f-103">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71c3f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71c3f-104">Prerequisites</span></span>
<span data-ttu-id="71c3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71c3f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71c3f-107">Permission type</span></span>|<span data-ttu-id="71c3f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71c3f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c3f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71c3f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71c3f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c3f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71c3f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71c3f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c3f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c3f-112">Not supported.</span></span>|
|<span data-ttu-id="71c3f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71c3f-113">Application</span></span>|<span data-ttu-id="71c3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c3f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c3f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71c3f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="71c3f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71c3f-116">Request headers</span></span>
|<span data-ttu-id="71c3f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71c3f-117">Header</span></span>|<span data-ttu-id="71c3f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="71c3f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c3f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71c3f-119">Authorization</span></span>|<span data-ttu-id="71c3f-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="71c3f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c3f-121">Принять</span><span class="sxs-lookup"><span data-stu-id="71c3f-121">Accept</span></span>|<span data-ttu-id="71c3f-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="71c3f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c3f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71c3f-123">Request body</span></span>
<span data-ttu-id="71c3f-124">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71c3f-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="71c3f-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="71c3f-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="71c3f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c3f-126">Property</span></span>|<span data-ttu-id="71c3f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="71c3f-127">Type</span></span>|<span data-ttu-id="71c3f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="71c3f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c3f-129">id</span><span class="sxs-lookup"><span data-stu-id="71c3f-129">id</span></span>|<span data-ttu-id="71c3f-130">Строка</span><span class="sxs-lookup"><span data-stu-id="71c3f-130">String</span></span>|<span data-ttu-id="71c3f-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71c3f-131">Key of the entity.</span></span>|
|<span data-ttu-id="71c3f-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="71c3f-132">pendingCount</span></span>|<span data-ttu-id="71c3f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-133">Int32</span></span>|<span data-ttu-id="71c3f-134">Количество ожидающих пользователей.</span><span class="sxs-lookup"><span data-stu-id="71c3f-134">Number of pending Users</span></span>|
|<span data-ttu-id="71c3f-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="71c3f-135">notApplicableCount</span></span>|<span data-ttu-id="71c3f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-136">Int32</span></span>|<span data-ttu-id="71c3f-137">Количество неприменимых пользователей</span><span class="sxs-lookup"><span data-stu-id="71c3f-137">Number of not applicable users.</span></span>|
|<span data-ttu-id="71c3f-138">successCount</span><span class="sxs-lookup"><span data-stu-id="71c3f-138">successCount</span></span>|<span data-ttu-id="71c3f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-139">Int32</span></span>|<span data-ttu-id="71c3f-140">Количество успешных пользователей.</span><span class="sxs-lookup"><span data-stu-id="71c3f-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="71c3f-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="71c3f-141">errorCount</span></span>|<span data-ttu-id="71c3f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-142">Int32</span></span>|<span data-ttu-id="71c3f-143">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="71c3f-143">Number of error Users</span></span>|
|<span data-ttu-id="71c3f-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="71c3f-144">failedCount</span></span>|<span data-ttu-id="71c3f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-145">Int32</span></span>|<span data-ttu-id="71c3f-146">Количество пользователей со сбоями.</span><span class="sxs-lookup"><span data-stu-id="71c3f-146">Number of failed Users</span></span>|
|<span data-ttu-id="71c3f-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="71c3f-147">lastUpdateDateTime</span></span>|<span data-ttu-id="71c3f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c3f-148">DateTimeOffset</span></span>|<span data-ttu-id="71c3f-149">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="71c3f-149">Last update time</span></span>|
|<span data-ttu-id="71c3f-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="71c3f-150">configurationVersion</span></span>|<span data-ttu-id="71c3f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="71c3f-151">Int32</span></span>|<span data-ttu-id="71c3f-152">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="71c3f-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="71c3f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c3f-153">Response</span></span>
<span data-ttu-id="71c3f-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71c3f-154">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c3f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="71c3f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="71c3f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c3f-156">Request</span></span>
<span data-ttu-id="71c3f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71c3f-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="71c3f-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="71c3f-158">Response</span></span>
<span data-ttu-id="71c3f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71c3f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








