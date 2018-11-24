# <a name="update-managedmobileapp"></a><span data-ttu-id="30e53-101">Обновление объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="30e53-101">Update managedMobileApp</span></span>

> <span data-ttu-id="30e53-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30e53-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30e53-103">Обновление свойств объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e53-103">Update the properties of a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30e53-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30e53-104">Prerequisites</span></span>
<span data-ttu-id="30e53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="30e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="30e53-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30e53-107">Permission type</span></span>|<span data-ttu-id="30e53-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30e53-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30e53-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30e53-109">Delegated (work or school account)</span></span>|<span data-ttu-id="30e53-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e53-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30e53-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30e53-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30e53-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e53-112">Not supported.</span></span>|
|<span data-ttu-id="30e53-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30e53-113">Application</span></span>|<span data-ttu-id="30e53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e53-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e53-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30e53-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="30e53-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30e53-116">Request headers</span></span>
|<span data-ttu-id="30e53-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30e53-117">Header</span></span>|<span data-ttu-id="30e53-118">Значение</span><span class="sxs-lookup"><span data-stu-id="30e53-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30e53-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="30e53-119">Authorization</span></span>|<span data-ttu-id="30e53-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30e53-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30e53-121">Accept</span><span class="sxs-lookup"><span data-stu-id="30e53-121">Accept</span></span>|<span data-ttu-id="30e53-122">application/json</span><span class="sxs-lookup"><span data-stu-id="30e53-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e53-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30e53-123">Request body</span></span>
<span data-ttu-id="30e53-124">В теле запроса добавьте представление объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30e53-124">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>

<span data-ttu-id="30e53-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e53-125">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span></span>

|<span data-ttu-id="30e53-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="30e53-126">Property</span></span>|<span data-ttu-id="30e53-127">Тип</span><span class="sxs-lookup"><span data-stu-id="30e53-127">Type</span></span>|<span data-ttu-id="30e53-128">Описание</span><span class="sxs-lookup"><span data-stu-id="30e53-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30e53-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="30e53-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="30e53-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="30e53-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="30e53-131">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="30e53-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="30e53-132">id</span><span class="sxs-lookup"><span data-stu-id="30e53-132">id</span></span>|<span data-ttu-id="30e53-133">String</span><span class="sxs-lookup"><span data-stu-id="30e53-133">String</span></span>|<span data-ttu-id="30e53-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30e53-134">Key of the entity.</span></span>|
|<span data-ttu-id="30e53-135">version</span><span class="sxs-lookup"><span data-stu-id="30e53-135">version</span></span>|<span data-ttu-id="30e53-136">String</span><span class="sxs-lookup"><span data-stu-id="30e53-136">String</span></span>|<span data-ttu-id="30e53-137">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="30e53-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="30e53-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="30e53-138">Response</span></span>
<span data-ttu-id="30e53-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedMobileApp](../resources/intune_mam_managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="30e53-139">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e53-140">Пример</span><span class="sxs-lookup"><span data-stu-id="30e53-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="30e53-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="30e53-141">Request</span></span>
<span data-ttu-id="30e53-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30e53-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="30e53-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="30e53-143">Response</span></span>
<span data-ttu-id="30e53-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="30e53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```



