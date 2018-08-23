# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="647ef-101">Создание объекта managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="647ef-101">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="647ef-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="647ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="647ef-103">Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="647ef-103">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="647ef-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="647ef-104">Prerequisites</span></span>
<span data-ttu-id="647ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="647ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="647ef-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="647ef-107">Permission type</span></span>|<span data-ttu-id="647ef-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="647ef-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="647ef-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="647ef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="647ef-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="647ef-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="647ef-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="647ef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="647ef-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="647ef-112">Not supported.</span></span>|
|<span data-ttu-id="647ef-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="647ef-113">Application</span></span>|<span data-ttu-id="647ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="647ef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="647ef-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="647ef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="647ef-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="647ef-116">Request headers</span></span>
|<span data-ttu-id="647ef-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="647ef-117">Header</span></span>|<span data-ttu-id="647ef-118">Значение</span><span class="sxs-lookup"><span data-stu-id="647ef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="647ef-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="647ef-119">Authorization</span></span>|<span data-ttu-id="647ef-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="647ef-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="647ef-121">Accept</span><span class="sxs-lookup"><span data-stu-id="647ef-121">Accept</span></span>|<span data-ttu-id="647ef-122">application/json</span><span class="sxs-lookup"><span data-stu-id="647ef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="647ef-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="647ef-123">Request body</span></span>
<span data-ttu-id="647ef-124">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="647ef-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="647ef-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="647ef-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="647ef-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="647ef-126">Property</span></span>|<span data-ttu-id="647ef-127">Тип</span><span class="sxs-lookup"><span data-stu-id="647ef-127">Type</span></span>|<span data-ttu-id="647ef-128">Описание</span><span class="sxs-lookup"><span data-stu-id="647ef-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="647ef-129">id</span><span class="sxs-lookup"><span data-stu-id="647ef-129">id</span></span>|<span data-ttu-id="647ef-130">string</span><span class="sxs-lookup"><span data-stu-id="647ef-130">String</span></span>|<span data-ttu-id="647ef-131">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="647ef-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="647ef-132">target</span><span class="sxs-lookup"><span data-stu-id="647ef-132">target</span></span>|[<span data-ttu-id="647ef-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="647ef-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="647ef-134">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="647ef-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="647ef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="647ef-135">Response</span></span>
<span data-ttu-id="647ef-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="647ef-136">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="647ef-137">Пример</span><span class="sxs-lookup"><span data-stu-id="647ef-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="647ef-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="647ef-138">Request</span></span>
<span data-ttu-id="647ef-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="647ef-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="647ef-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="647ef-140">Response</span></span>
<span data-ttu-id="647ef-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="647ef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



