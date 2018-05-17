# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="32470-101">Обновление объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="32470-101">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="32470-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32470-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32470-103">Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32470-103">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32470-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32470-104">Prerequisites</span></span>
<span data-ttu-id="32470-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32470-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32470-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32470-107">Permission type</span></span>|<span data-ttu-id="32470-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32470-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32470-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32470-109">Delegated (work or school account)</span></span>|<span data-ttu-id="32470-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32470-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32470-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32470-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32470-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32470-112">Not supported.</span></span>|
|<span data-ttu-id="32470-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32470-113">Application</span></span>|<span data-ttu-id="32470-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32470-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32470-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32470-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="32470-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32470-116">Request headers</span></span>
|<span data-ttu-id="32470-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32470-117">Header</span></span>|<span data-ttu-id="32470-118">Значение</span><span class="sxs-lookup"><span data-stu-id="32470-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32470-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="32470-119">Authorization</span></span>|<span data-ttu-id="32470-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32470-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32470-121">Accept</span><span class="sxs-lookup"><span data-stu-id="32470-121">Accept</span></span>|<span data-ttu-id="32470-122">application/json</span><span class="sxs-lookup"><span data-stu-id="32470-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32470-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32470-123">Request body</span></span>
<span data-ttu-id="32470-124">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32470-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="32470-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32470-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="32470-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="32470-126">Property</span></span>|<span data-ttu-id="32470-127">Тип</span><span class="sxs-lookup"><span data-stu-id="32470-127">Type</span></span>|<span data-ttu-id="32470-128">Описание</span><span class="sxs-lookup"><span data-stu-id="32470-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32470-129">id</span><span class="sxs-lookup"><span data-stu-id="32470-129">id</span></span>|<span data-ttu-id="32470-130">String</span><span class="sxs-lookup"><span data-stu-id="32470-130">String</span></span>|<span data-ttu-id="32470-131">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="32470-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="32470-132">target</span><span class="sxs-lookup"><span data-stu-id="32470-132">target</span></span>|[<span data-ttu-id="32470-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="32470-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="32470-134">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="32470-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="32470-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="32470-135">Response</span></span>
<span data-ttu-id="32470-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32470-136">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32470-137">Пример</span><span class="sxs-lookup"><span data-stu-id="32470-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="32470-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="32470-138">Request</span></span>
<span data-ttu-id="32470-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32470-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="32470-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="32470-140">Response</span></span>
<span data-ttu-id="32470-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="32470-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



