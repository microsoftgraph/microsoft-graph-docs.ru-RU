# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="79f27-101">Создание объекта deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="79f27-101">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="79f27-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="79f27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79f27-103">Создание объекта [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="79f27-103">Create a new [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79f27-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="79f27-104">Prerequisites</span></span>
<span data-ttu-id="79f27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79f27-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79f27-107">Permission type</span></span>|<span data-ttu-id="79f27-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="79f27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79f27-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79f27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79f27-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79f27-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79f27-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79f27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f27-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f27-112">Not supported.</span></span>|
|<span data-ttu-id="79f27-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79f27-113">Application</span></span>|<span data-ttu-id="79f27-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79f27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79f27-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79f27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="79f27-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79f27-116">Request headers</span></span>
|<span data-ttu-id="79f27-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79f27-117">Header</span></span>|<span data-ttu-id="79f27-118">Значение</span><span class="sxs-lookup"><span data-stu-id="79f27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79f27-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="79f27-119">Authorization</span></span>|<span data-ttu-id="79f27-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79f27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79f27-121">Accept</span><span class="sxs-lookup"><span data-stu-id="79f27-121">Accept</span></span>|<span data-ttu-id="79f27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="79f27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f27-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79f27-123">Request body</span></span>
<span data-ttu-id="79f27-124">В тексте запроса добавьте представление объекта deviceCompliancePolicyAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79f27-124">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="79f27-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="79f27-125">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="79f27-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="79f27-126">Property</span></span>|<span data-ttu-id="79f27-127">Тип</span><span class="sxs-lookup"><span data-stu-id="79f27-127">Type</span></span>|<span data-ttu-id="79f27-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79f27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f27-129">id</span><span class="sxs-lookup"><span data-stu-id="79f27-129">id</span></span>|<span data-ttu-id="79f27-130">String</span><span class="sxs-lookup"><span data-stu-id="79f27-130">String</span></span>|<span data-ttu-id="79f27-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79f27-131">Key of the entity.</span></span>|
|<span data-ttu-id="79f27-132">target</span><span class="sxs-lookup"><span data-stu-id="79f27-132">target</span></span>|[<span data-ttu-id="79f27-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="79f27-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="79f27-134">Цель для назначения политики соответствия.</span><span class="sxs-lookup"><span data-stu-id="79f27-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="79f27-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="79f27-135">Response</span></span>
<span data-ttu-id="79f27-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79f27-136">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f27-137">Пример</span><span class="sxs-lookup"><span data-stu-id="79f27-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="79f27-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="79f27-138">Request</span></span>
<span data-ttu-id="79f27-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79f27-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="79f27-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="79f27-140">Response</span></span>
<span data-ttu-id="79f27-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="79f27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



