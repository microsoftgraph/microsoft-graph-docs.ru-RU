# <a name="create-managedmobileapp"></a><span data-ttu-id="fe237-101">Создание объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="fe237-101">Create managedMobileApp</span></span>

> <span data-ttu-id="fe237-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe237-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe237-103">Создание объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe237-103">Create a new [plannerBucket](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe237-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe237-104">Prerequisites</span></span>
<span data-ttu-id="fe237-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fe237-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe237-107">Permission type</span></span>|<span data-ttu-id="fe237-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe237-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe237-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe237-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fe237-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe237-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe237-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe237-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe237-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe237-112">Not supported.</span></span>|
|<span data-ttu-id="fe237-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe237-113">Application</span></span>|<span data-ttu-id="fe237-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe237-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe237-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe237-115">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fe237-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe237-116">Request headers</span></span>
|<span data-ttu-id="fe237-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe237-117">Header</span></span>|<span data-ttu-id="fe237-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fe237-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe237-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe237-119">Authorization</span></span>|<span data-ttu-id="fe237-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe237-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe237-121">Accept</span><span class="sxs-lookup"><span data-stu-id="fe237-121">Accept</span></span>|<span data-ttu-id="fe237-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fe237-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe237-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe237-123">Request body</span></span>
<span data-ttu-id="fe237-124">В теле запроса добавьте представление объекта managedMobileApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe237-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="fe237-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedMobileApp.</span><span class="sxs-lookup"><span data-stu-id="fe237-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="fe237-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe237-126">Property</span></span>|<span data-ttu-id="fe237-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fe237-127">Type</span></span>|<span data-ttu-id="fe237-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fe237-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe237-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe237-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="fe237-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe237-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="fe237-131">Идентификатор приложения с типом его операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fe237-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="fe237-132">id</span><span class="sxs-lookup"><span data-stu-id="fe237-132">id</span></span>|<span data-ttu-id="fe237-133">String</span><span class="sxs-lookup"><span data-stu-id="fe237-133">String</span></span>|<span data-ttu-id="fe237-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe237-134">Key of the setting.</span></span>|
|<span data-ttu-id="fe237-135">version</span><span class="sxs-lookup"><span data-stu-id="fe237-135">version</span></span>|<span data-ttu-id="fe237-136">String</span><span class="sxs-lookup"><span data-stu-id="fe237-136">String</span></span>|<span data-ttu-id="fe237-137">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="fe237-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fe237-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe237-138">Response</span></span>
<span data-ttu-id="fe237-139">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [managedMobileApp](../resources/intune_mam_managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe237-139">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe237-140">Пример</span><span class="sxs-lookup"><span data-stu-id="fe237-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe237-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe237-141">Request</span></span>
<span data-ttu-id="fe237-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe237-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe237-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe237-143">Response</span></span>
<span data-ttu-id="fe237-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe237-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



