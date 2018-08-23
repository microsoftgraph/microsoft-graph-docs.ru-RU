# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="b74d7-101">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="b74d7-101">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="b74d7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b74d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b74d7-103">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b74d7-103">Update the properties of a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b74d7-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b74d7-104">Prerequisites</span></span>
<span data-ttu-id="b74d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b74d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b74d7-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b74d7-107">Permission type</span></span>|<span data-ttu-id="b74d7-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b74d7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b74d7-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b74d7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b74d7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b74d7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b74d7-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b74d7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b74d7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b74d7-112">Not supported.</span></span>|
|<span data-ttu-id="b74d7-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b74d7-113">Application</span></span>|<span data-ttu-id="b74d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b74d7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b74d7-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b74d7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b74d7-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b74d7-116">Request headers</span></span>
|<span data-ttu-id="b74d7-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b74d7-117">Header</span></span>|<span data-ttu-id="b74d7-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b74d7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b74d7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b74d7-119">Authorization</span></span>|<span data-ttu-id="b74d7-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b74d7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b74d7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b74d7-121">Accept</span></span>|<span data-ttu-id="b74d7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b74d7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b74d7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b74d7-123">Request body</span></span>
<span data-ttu-id="b74d7-124">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b74d7-124">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="b74d7-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b74d7-125">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="b74d7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b74d7-126">Property</span></span>|<span data-ttu-id="b74d7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b74d7-127">Type</span></span>|<span data-ttu-id="b74d7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b74d7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b74d7-129">id</span><span class="sxs-lookup"><span data-stu-id="b74d7-129">id</span></span>|<span data-ttu-id="b74d7-130">string</span><span class="sxs-lookup"><span data-stu-id="b74d7-130">String</span></span>|<span data-ttu-id="b74d7-131">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="b74d7-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b74d7-132">target</span><span class="sxs-lookup"><span data-stu-id="b74d7-132">target</span></span>|[<span data-ttu-id="b74d7-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b74d7-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b74d7-134">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="b74d7-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="b74d7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b74d7-135">Response</span></span>
<span data-ttu-id="b74d7-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b74d7-136">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b74d7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b74d7-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="b74d7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b74d7-138">Request</span></span>
<span data-ttu-id="b74d7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b74d7-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b74d7-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b74d7-140">Response</span></span>
<span data-ttu-id="b74d7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b74d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



