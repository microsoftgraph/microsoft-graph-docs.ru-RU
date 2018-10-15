# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="637b3-101">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="637b3-101">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="637b3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="637b3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="637b3-103">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="637b3-103">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="637b3-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="637b3-104">Prerequisites</span></span>
<span data-ttu-id="637b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="637b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="637b3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="637b3-107">Permission type</span></span>|<span data-ttu-id="637b3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="637b3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="637b3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="637b3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="637b3-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="637b3-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="637b3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="637b3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="637b3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="637b3-112">Not supported.</span></span>|
|<span data-ttu-id="637b3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="637b3-113">Application</span></span>|<span data-ttu-id="637b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="637b3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="637b3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="637b3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="637b3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="637b3-116">Request headers</span></span>
|<span data-ttu-id="637b3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="637b3-117">Header</span></span>|<span data-ttu-id="637b3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="637b3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="637b3-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="637b3-119">Authorization</span></span>|<span data-ttu-id="637b3-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="637b3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="637b3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="637b3-121">Accept</span></span>|<span data-ttu-id="637b3-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="637b3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="637b3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="637b3-123">Request body</span></span>
<span data-ttu-id="637b3-124">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="637b3-124">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="637b3-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="637b3-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="637b3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="637b3-126">Property</span></span>|<span data-ttu-id="637b3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="637b3-127">Type</span></span>|<span data-ttu-id="637b3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="637b3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="637b3-129">id</span><span class="sxs-lookup"><span data-stu-id="637b3-129">id</span></span>|<span data-ttu-id="637b3-130">Строка</span><span class="sxs-lookup"><span data-stu-id="637b3-130">String</span></span>|<span data-ttu-id="637b3-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="637b3-131">Not yet documented</span></span>|
|<span data-ttu-id="637b3-132">target</span><span class="sxs-lookup"><span data-stu-id="637b3-132">target</span></span>|[<span data-ttu-id="637b3-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="637b3-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="637b3-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="637b3-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="637b3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="637b3-135">Response</span></span>
<span data-ttu-id="637b3-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="637b3-136">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="637b3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="637b3-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="637b3-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="637b3-138">Request</span></span>
<span data-ttu-id="637b3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="637b3-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="637b3-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="637b3-140">Response</span></span>
<span data-ttu-id="637b3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="637b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








