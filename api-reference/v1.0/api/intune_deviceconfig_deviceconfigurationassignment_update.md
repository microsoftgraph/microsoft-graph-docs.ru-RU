# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="48c5c-101">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="48c5c-101">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="48c5c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="48c5c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48c5c-103">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="48c5c-103">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48c5c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="48c5c-104">Prerequisites</span></span>
<span data-ttu-id="48c5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="48c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48c5c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48c5c-107">Permission type</span></span>|<span data-ttu-id="48c5c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48c5c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48c5c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48c5c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="48c5c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48c5c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48c5c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48c5c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48c5c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48c5c-112">Not supported.</span></span>|
|<span data-ttu-id="48c5c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48c5c-113">Application</span></span>|<span data-ttu-id="48c5c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48c5c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48c5c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48c5c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="48c5c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48c5c-116">Request headers</span></span>
|<span data-ttu-id="48c5c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48c5c-117">Header</span></span>|<span data-ttu-id="48c5c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="48c5c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48c5c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="48c5c-119">Authorization</span></span>|<span data-ttu-id="48c5c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48c5c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48c5c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="48c5c-121">Accept</span></span>|<span data-ttu-id="48c5c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="48c5c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48c5c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48c5c-123">Request body</span></span>
<span data-ttu-id="48c5c-124">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48c5c-124">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="48c5c-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="48c5c-125">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="48c5c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="48c5c-126">Property</span></span>|<span data-ttu-id="48c5c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="48c5c-127">Type</span></span>|<span data-ttu-id="48c5c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="48c5c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48c5c-129">id</span><span class="sxs-lookup"><span data-stu-id="48c5c-129">id</span></span>|<span data-ttu-id="48c5c-130">String</span><span class="sxs-lookup"><span data-stu-id="48c5c-130">String</span></span>|<span data-ttu-id="48c5c-131">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="48c5c-131">The key of the assignment.</span></span>|
|<span data-ttu-id="48c5c-132">target</span><span class="sxs-lookup"><span data-stu-id="48c5c-132">target</span></span>|[<span data-ttu-id="48c5c-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="48c5c-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="48c5c-134">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="48c5c-134">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="48c5c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="48c5c-135">Response</span></span>
<span data-ttu-id="48c5c-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48c5c-136">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48c5c-137">Пример</span><span class="sxs-lookup"><span data-stu-id="48c5c-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="48c5c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="48c5c-138">Request</span></span>
<span data-ttu-id="48c5c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48c5c-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="48c5c-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="48c5c-140">Response</span></span>
<span data-ttu-id="48c5c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48c5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



