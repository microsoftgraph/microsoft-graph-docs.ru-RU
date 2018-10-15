# <a name="update-managedappoperation"></a><span data-ttu-id="4be14-101">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="4be14-101">Update managedAppOperation</span></span>

> <span data-ttu-id="4be14-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4be14-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4be14-103">Обновление свойств объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4be14-103">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4be14-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4be14-104">Prerequisites</span></span>
<span data-ttu-id="4be14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4be14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4be14-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4be14-107">Permission type</span></span>|<span data-ttu-id="4be14-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4be14-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4be14-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4be14-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4be14-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be14-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4be14-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4be14-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4be14-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be14-112">Not supported.</span></span>|
|<span data-ttu-id="4be14-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4be14-113">Application</span></span>|<span data-ttu-id="4be14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4be14-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4be14-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4be14-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="4be14-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4be14-116">Request headers</span></span>
|<span data-ttu-id="4be14-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4be14-117">Header</span></span>|<span data-ttu-id="4be14-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4be14-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4be14-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4be14-119">Authorization</span></span>|<span data-ttu-id="4be14-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="4be14-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4be14-121">Принять</span><span class="sxs-lookup"><span data-stu-id="4be14-121">Accept</span></span>|<span data-ttu-id="4be14-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4be14-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4be14-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4be14-123">Request body</span></span>
<span data-ttu-id="4be14-124">В теле запроса добавьте представление объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4be14-124">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>

<span data-ttu-id="4be14-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4be14-125">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>

|<span data-ttu-id="4be14-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be14-126">Property</span></span>|<span data-ttu-id="4be14-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4be14-127">Type</span></span>|<span data-ttu-id="4be14-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4be14-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be14-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4be14-129">displayName</span></span>|<span data-ttu-id="4be14-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4be14-130">String</span></span>|<span data-ttu-id="4be14-131">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="4be14-131">The operation name.</span></span>|
|<span data-ttu-id="4be14-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4be14-132">lastModifiedDateTime</span></span>|<span data-ttu-id="4be14-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4be14-133">DateTimeOffset</span></span>|<span data-ttu-id="4be14-134">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="4be14-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="4be14-135">state</span><span class="sxs-lookup"><span data-stu-id="4be14-135">state</span></span>|<span data-ttu-id="4be14-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4be14-136">String</span></span>|<span data-ttu-id="4be14-137">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="4be14-137">The current state of the operation</span></span>|
|<span data-ttu-id="4be14-138">id</span><span class="sxs-lookup"><span data-stu-id="4be14-138">id</span></span>|<span data-ttu-id="4be14-139">Строка</span><span class="sxs-lookup"><span data-stu-id="4be14-139">String</span></span>|<span data-ttu-id="4be14-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4be14-140">Key of the entity.</span></span>|
|<span data-ttu-id="4be14-141">version</span><span class="sxs-lookup"><span data-stu-id="4be14-141">version</span></span>|<span data-ttu-id="4be14-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4be14-142">String</span></span>|<span data-ttu-id="4be14-143">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="4be14-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4be14-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4be14-144">Response</span></span>
<span data-ttu-id="4be14-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppOperation](../resources/intune_mam_managedappoperation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4be14-145">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4be14-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4be14-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="4be14-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4be14-147">Request</span></span>
<span data-ttu-id="4be14-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4be14-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4be14-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="4be14-149">Response</span></span>
<span data-ttu-id="4be14-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4be14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```








