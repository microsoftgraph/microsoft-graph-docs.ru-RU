# <a name="create-managedmobileapp"></a><span data-ttu-id="8e552-101">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="8e552-101">Create managedMobileApp</span></span>

> <span data-ttu-id="8e552-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e552-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e552-103">Создание объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e552-103">Create a new [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e552-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e552-104">Prerequisites</span></span>
<span data-ttu-id="8e552-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e552-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e552-107">Permission type</span></span>|<span data-ttu-id="8e552-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e552-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e552-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e552-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8e552-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e552-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e552-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e552-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e552-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e552-112">Not supported.</span></span>|
|<span data-ttu-id="8e552-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e552-113">Application</span></span>|<span data-ttu-id="8e552-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e552-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e552-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e552-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="8e552-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e552-116">Request headers</span></span>
|<span data-ttu-id="8e552-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e552-117">Header</span></span>|<span data-ttu-id="8e552-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8e552-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e552-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e552-119">Authorization</span></span>|<span data-ttu-id="8e552-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8e552-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e552-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8e552-121">Accept</span></span>|<span data-ttu-id="8e552-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8e552-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e552-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e552-123">Request body</span></span>
<span data-ttu-id="8e552-124">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e552-124">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="8e552-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="8e552-125">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="8e552-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e552-126">Property</span></span>|<span data-ttu-id="8e552-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8e552-127">Type</span></span>|<span data-ttu-id="8e552-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8e552-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e552-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e552-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="8e552-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e552-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="8e552-131">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8e552-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="8e552-132">id</span><span class="sxs-lookup"><span data-stu-id="8e552-132">id</span></span>|<span data-ttu-id="8e552-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8e552-133">String</span></span>|<span data-ttu-id="8e552-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e552-134">Key of the entity.</span></span>|
|<span data-ttu-id="8e552-135">version</span><span class="sxs-lookup"><span data-stu-id="8e552-135">version</span></span>|<span data-ttu-id="8e552-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8e552-136">String</span></span>|<span data-ttu-id="8e552-137">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8e552-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8e552-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e552-138">Response</span></span>
<span data-ttu-id="8e552-139">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune_mam_managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e552-139">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e552-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8e552-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e552-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e552-141">Request</span></span>
<span data-ttu-id="8e552-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e552-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="8e552-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e552-143">Response</span></span>
<span data-ttu-id="8e552-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








