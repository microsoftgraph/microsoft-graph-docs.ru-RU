# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="12bf1-101">Создание targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="12bf1-101">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="12bf1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12bf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12bf1-103">Создание объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-103">Create a new [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12bf1-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12bf1-104">Prerequisites</span></span>
<span data-ttu-id="12bf1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12bf1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12bf1-107">Permission type</span></span>|<span data-ttu-id="12bf1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12bf1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12bf1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12bf1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12bf1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12bf1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12bf1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12bf1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12bf1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12bf1-112">Not supported.</span></span>|
|<span data-ttu-id="12bf1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12bf1-113">Application</span></span>|<span data-ttu-id="12bf1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12bf1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12bf1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12bf1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12bf1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12bf1-116">Request headers</span></span>
|<span data-ttu-id="12bf1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12bf1-117">Header</span></span>|<span data-ttu-id="12bf1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="12bf1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12bf1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12bf1-119">Authorization</span></span>|<span data-ttu-id="12bf1-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="12bf1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12bf1-121">Принять</span><span class="sxs-lookup"><span data-stu-id="12bf1-121">Accept</span></span>|<span data-ttu-id="12bf1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="12bf1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12bf1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12bf1-123">Request body</span></span>
<span data-ttu-id="12bf1-124">В теле запроса добавьте представление объекта targetedManagedAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12bf1-124">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="12bf1-125">Ниже показаны свойства, которые необходимо указывать при создании объекта targetedManagedAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="12bf1-125">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="12bf1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="12bf1-126">Property</span></span>|<span data-ttu-id="12bf1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="12bf1-127">Type</span></span>|<span data-ttu-id="12bf1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="12bf1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12bf1-129">displayName</span><span class="sxs-lookup"><span data-stu-id="12bf1-129">displayName</span></span>|<span data-ttu-id="12bf1-130">Строка</span><span class="sxs-lookup"><span data-stu-id="12bf1-130">String</span></span>|<span data-ttu-id="12bf1-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="12bf1-131">Policy display name.</span></span> <span data-ttu-id="12bf1-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-133">description</span><span class="sxs-lookup"><span data-stu-id="12bf1-133">description</span></span>|<span data-ttu-id="12bf1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="12bf1-134">String</span></span>|<span data-ttu-id="12bf1-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="12bf1-135">The policy's description.</span></span> <span data-ttu-id="12bf1-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12bf1-137">createdDateTime</span></span>|<span data-ttu-id="12bf1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12bf1-138">DateTimeOffset</span></span>|<span data-ttu-id="12bf1-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="12bf1-139">The date and time the policy was created.</span></span> <span data-ttu-id="12bf1-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12bf1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="12bf1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12bf1-142">DateTimeOffset</span></span>|<span data-ttu-id="12bf1-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="12bf1-143">Last time the policy was modified.</span></span> <span data-ttu-id="12bf1-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-145">id</span><span class="sxs-lookup"><span data-stu-id="12bf1-145">id</span></span>|<span data-ttu-id="12bf1-146">Строка</span><span class="sxs-lookup"><span data-stu-id="12bf1-146">String</span></span>|<span data-ttu-id="12bf1-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12bf1-147">Key of the entity.</span></span> <span data-ttu-id="12bf1-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-149">version</span><span class="sxs-lookup"><span data-stu-id="12bf1-149">version</span></span>|<span data-ttu-id="12bf1-150">Строка</span><span class="sxs-lookup"><span data-stu-id="12bf1-150">String</span></span>|<span data-ttu-id="12bf1-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="12bf1-151">Version of the entity.</span></span> <span data-ttu-id="12bf1-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="12bf1-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="12bf1-153">customSettings</span></span>|<span data-ttu-id="12bf1-154">Коллекция [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="12bf1-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="12bf1-155">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12bf1-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="12bf1-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="12bf1-156">deployedAppCount</span></span>|<span data-ttu-id="12bf1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="12bf1-157">Int32</span></span>|<span data-ttu-id="12bf1-158">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="12bf1-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="12bf1-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="12bf1-159">isAssigned</span></span>|<span data-ttu-id="12bf1-160">Логический</span><span class="sxs-lookup"><span data-stu-id="12bf1-160">Boolean</span></span>|<span data-ttu-id="12bf1-161">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="12bf1-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="12bf1-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="12bf1-162">Response</span></span>
<span data-ttu-id="12bf1-163">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12bf1-163">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12bf1-164">Пример</span><span class="sxs-lookup"><span data-stu-id="12bf1-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="12bf1-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="12bf1-165">Request</span></span>
<span data-ttu-id="12bf1-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12bf1-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="12bf1-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="12bf1-167">Response</span></span>
<span data-ttu-id="12bf1-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12bf1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```








