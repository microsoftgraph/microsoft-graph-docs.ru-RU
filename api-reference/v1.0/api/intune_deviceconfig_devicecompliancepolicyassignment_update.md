# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="228cb-101">Обновление объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="228cb-101">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="228cb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="228cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="228cb-103">Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="228cb-103">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="228cb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="228cb-104">Prerequisites</span></span>
<span data-ttu-id="228cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="228cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="228cb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="228cb-107">Permission type</span></span>|<span data-ttu-id="228cb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="228cb-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="228cb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228cb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="228cb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228cb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="228cb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228cb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="228cb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228cb-112">Not supported.</span></span>|
|<span data-ttu-id="228cb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="228cb-113">Application</span></span>|<span data-ttu-id="228cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228cb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="228cb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228cb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="228cb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="228cb-116">Request headers</span></span>
|<span data-ttu-id="228cb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="228cb-117">Header</span></span>|<span data-ttu-id="228cb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="228cb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="228cb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="228cb-119">Authorization</span></span>|<span data-ttu-id="228cb-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="228cb-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="228cb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="228cb-121">Accept</span></span>|<span data-ttu-id="228cb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="228cb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="228cb-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="228cb-123">Request body</span></span>
<span data-ttu-id="228cb-124">В тексте запроса добавьте представление объекта [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="228cb-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="228cb-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="228cb-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="228cb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="228cb-126">Property</span></span>|<span data-ttu-id="228cb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="228cb-127">Type</span></span>|<span data-ttu-id="228cb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="228cb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="228cb-129">id</span><span class="sxs-lookup"><span data-stu-id="228cb-129">id</span></span>|<span data-ttu-id="228cb-130">String</span><span class="sxs-lookup"><span data-stu-id="228cb-130">String</span></span>|<span data-ttu-id="228cb-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="228cb-131">Key of the entity.</span></span>|
|<span data-ttu-id="228cb-132">target</span><span class="sxs-lookup"><span data-stu-id="228cb-132">target</span></span>|[<span data-ttu-id="228cb-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="228cb-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="228cb-134">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="228cb-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="228cb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="228cb-135">Response</span></span>
<span data-ttu-id="228cb-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="228cb-136">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="228cb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="228cb-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="228cb-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="228cb-138">Request</span></span>
<span data-ttu-id="228cb-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="228cb-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="228cb-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="228cb-140">Response</span></span>
<span data-ttu-id="228cb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="228cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



