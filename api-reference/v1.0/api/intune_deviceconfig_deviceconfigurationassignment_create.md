# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="09305-101">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="09305-101">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="09305-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09305-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09305-103">Создание объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09305-103">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09305-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="09305-104">Prerequisites</span></span>
<span data-ttu-id="09305-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="09305-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09305-107">Permission type</span></span>|<span data-ttu-id="09305-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09305-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09305-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09305-109">Delegated (work or school account)</span></span>|<span data-ttu-id="09305-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09305-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09305-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09305-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09305-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09305-112">Not supported.</span></span>|
|<span data-ttu-id="09305-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09305-113">Application</span></span>|<span data-ttu-id="09305-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09305-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09305-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09305-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="09305-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09305-116">Request headers</span></span>
|<span data-ttu-id="09305-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09305-117">Header</span></span>|<span data-ttu-id="09305-118">Значение</span><span class="sxs-lookup"><span data-stu-id="09305-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09305-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="09305-119">Authorization</span></span>|<span data-ttu-id="09305-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09305-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09305-121">Accept</span><span class="sxs-lookup"><span data-stu-id="09305-121">Accept</span></span>|<span data-ttu-id="09305-122">application/json</span><span class="sxs-lookup"><span data-stu-id="09305-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09305-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09305-123">Request body</span></span>
<span data-ttu-id="09305-124">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09305-124">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="09305-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="09305-125">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="09305-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="09305-126">Property</span></span>|<span data-ttu-id="09305-127">Тип</span><span class="sxs-lookup"><span data-stu-id="09305-127">Type</span></span>|<span data-ttu-id="09305-128">Описание</span><span class="sxs-lookup"><span data-stu-id="09305-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09305-129">id</span><span class="sxs-lookup"><span data-stu-id="09305-129">id</span></span>|<span data-ttu-id="09305-130">String</span><span class="sxs-lookup"><span data-stu-id="09305-130">String</span></span>|<span data-ttu-id="09305-131">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="09305-131">The key of the assignment.</span></span>|
|<span data-ttu-id="09305-132">target</span><span class="sxs-lookup"><span data-stu-id="09305-132">target</span></span>|[<span data-ttu-id="09305-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="09305-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="09305-134">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="09305-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="09305-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="09305-135">Response</span></span>
<span data-ttu-id="09305-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09305-136">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09305-137">Пример</span><span class="sxs-lookup"><span data-stu-id="09305-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="09305-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="09305-138">Request</span></span>
<span data-ttu-id="09305-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09305-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="09305-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="09305-140">Response</span></span>
<span data-ttu-id="09305-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="09305-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



