# <a name="update-mobileappassignment"></a><span data-ttu-id="435e5-101">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="435e5-101">Update mobileAppAssignment</span></span>

> <span data-ttu-id="435e5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="435e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="435e5-103">Обновление свойств объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="435e5-103">Update the properties of a [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="435e5-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="435e5-104">Prerequisites</span></span>
<span data-ttu-id="435e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="435e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="435e5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="435e5-107">Permission type</span></span>|<span data-ttu-id="435e5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="435e5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="435e5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="435e5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="435e5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="435e5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="435e5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="435e5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="435e5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="435e5-112">Not supported.</span></span>|
|<span data-ttu-id="435e5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="435e5-113">Application</span></span>|<span data-ttu-id="435e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="435e5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="435e5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="435e5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="435e5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="435e5-116">Request headers</span></span>
|<span data-ttu-id="435e5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="435e5-117">Header</span></span>|<span data-ttu-id="435e5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="435e5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="435e5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="435e5-119">Authorization</span></span>|<span data-ttu-id="435e5-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="435e5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="435e5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="435e5-121">Accept</span></span>|<span data-ttu-id="435e5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="435e5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="435e5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="435e5-123">Request body</span></span>
<span data-ttu-id="435e5-124">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="435e5-124">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object.</span></span>

<span data-ttu-id="435e5-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="435e5-125">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span></span>

|<span data-ttu-id="435e5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="435e5-126">Property</span></span>|<span data-ttu-id="435e5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="435e5-127">Type</span></span>|<span data-ttu-id="435e5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="435e5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="435e5-129">id</span><span class="sxs-lookup"><span data-stu-id="435e5-129">id</span></span>|<span data-ttu-id="435e5-130">String</span><span class="sxs-lookup"><span data-stu-id="435e5-130">String</span></span>|<span data-ttu-id="435e5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="435e5-131">Key of the entity.</span></span>|
|<span data-ttu-id="435e5-132">intent</span><span class="sxs-lookup"><span data-stu-id="435e5-132">intent</span></span>|[<span data-ttu-id="435e5-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="435e5-133">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="435e5-134">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="435e5-134">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="435e5-135">target</span><span class="sxs-lookup"><span data-stu-id="435e5-135">target</span></span>|[<span data-ttu-id="435e5-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="435e5-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="435e5-137">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="435e5-137">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="435e5-138">settings</span><span class="sxs-lookup"><span data-stu-id="435e5-138">settings</span></span>|[<span data-ttu-id="435e5-139">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="435e5-139">mobileAppAssignmentSettings</span></span>](../resources/intune_apps_mobileappassignmentsettings.md)|<span data-ttu-id="435e5-140">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="435e5-140">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="435e5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="435e5-141">Response</span></span>
<span data-ttu-id="435e5-142">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="435e5-142">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="435e5-143">Пример</span><span class="sxs-lookup"><span data-stu-id="435e5-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="435e5-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="435e5-144">Request</span></span>
<span data-ttu-id="435e5-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="435e5-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="435e5-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="435e5-146">Response</span></span>
<span data-ttu-id="435e5-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="435e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



