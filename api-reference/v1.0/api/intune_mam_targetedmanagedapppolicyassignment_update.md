# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="40122-101">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="40122-101">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="40122-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40122-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40122-103">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="40122-103">Update the properties of a [calendar](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40122-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="40122-104">Prerequisites</span></span>
<span data-ttu-id="40122-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="40122-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40122-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40122-107">Permission type</span></span>|<span data-ttu-id="40122-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40122-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40122-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40122-109">Delegated (work or school account)</span></span>|<span data-ttu-id="40122-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40122-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40122-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40122-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40122-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40122-112">Not supported.</span></span>|
|<span data-ttu-id="40122-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40122-113">Application</span></span>|<span data-ttu-id="40122-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40122-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40122-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40122-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="40122-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40122-116">Request headers</span></span>
|<span data-ttu-id="40122-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40122-117">Header</span></span>|<span data-ttu-id="40122-118">Значение</span><span class="sxs-lookup"><span data-stu-id="40122-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40122-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="40122-119">Authorization</span></span>|<span data-ttu-id="40122-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40122-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="40122-121">Accept</span><span class="sxs-lookup"><span data-stu-id="40122-121">Accept</span></span>|<span data-ttu-id="40122-122">application/json</span><span class="sxs-lookup"><span data-stu-id="40122-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40122-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40122-123">Request body</span></span>
<span data-ttu-id="40122-124">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40122-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="40122-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="40122-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="40122-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="40122-126">Property</span></span>|<span data-ttu-id="40122-127">Тип</span><span class="sxs-lookup"><span data-stu-id="40122-127">Type</span></span>|<span data-ttu-id="40122-128">Описание</span><span class="sxs-lookup"><span data-stu-id="40122-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40122-129">id</span><span class="sxs-lookup"><span data-stu-id="40122-129">id</span></span>|<span data-ttu-id="40122-130">String</span><span class="sxs-lookup"><span data-stu-id="40122-130">String</span></span>|<span data-ttu-id="40122-131">Id</span><span class="sxs-lookup"><span data-stu-id="40122-131">Id</span></span>|
|<span data-ttu-id="40122-132">target</span><span class="sxs-lookup"><span data-stu-id="40122-132">target</span></span>|[<span data-ttu-id="40122-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="40122-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="40122-134">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="40122-134">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="40122-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40122-135">Response</span></span>
<span data-ttu-id="40122-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40122-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40122-137">Пример</span><span class="sxs-lookup"><span data-stu-id="40122-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="40122-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="40122-138">Request</span></span>
<span data-ttu-id="40122-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40122-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="40122-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="40122-140">Response</span></span>
<span data-ttu-id="40122-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40122-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



