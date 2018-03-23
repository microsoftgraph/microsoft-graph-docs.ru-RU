# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="2f1ae-101">Обновление объекта targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f1ae-101">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="2f1ae-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f1ae-103">Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-103">Update the properties of a [calendar](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f1ae-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f1ae-104">Prerequisites</span></span>
<span data-ttu-id="2f1ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f1ae-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f1ae-107">Permission type</span></span>|<span data-ttu-id="2f1ae-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f1ae-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2f1ae-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f1ae-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f1ae-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f1ae-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-112">Not supported.</span></span>|
|<span data-ttu-id="2f1ae-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f1ae-113">Application</span></span>|<span data-ttu-id="2f1ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f1ae-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f1ae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2f1ae-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f1ae-116">Request headers</span></span>
|<span data-ttu-id="2f1ae-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f1ae-117">Header</span></span>|<span data-ttu-id="2f1ae-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2f1ae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f1ae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f1ae-119">Authorization</span></span>|<span data-ttu-id="2f1ae-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2f1ae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2f1ae-121">Accept</span></span>|<span data-ttu-id="2f1ae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2f1ae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f1ae-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f1ae-123">Request body</span></span>
<span data-ttu-id="2f1ae-124">В теле запроса добавьте представление объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="2f1ae-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2f1ae-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f1ae-126">Property</span></span>|<span data-ttu-id="2f1ae-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2f1ae-127">Type</span></span>|<span data-ttu-id="2f1ae-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2f1ae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f1ae-129">displayName</span><span class="sxs-lookup"><span data-stu-id="2f1ae-129">displayName</span></span>|<span data-ttu-id="2f1ae-130">String</span><span class="sxs-lookup"><span data-stu-id="2f1ae-130">String</span></span>|<span data-ttu-id="2f1ae-131">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-131">Policy display name.</span></span> <span data-ttu-id="2f1ae-132">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-133">description</span><span class="sxs-lookup"><span data-stu-id="2f1ae-133">description</span></span>|<span data-ttu-id="2f1ae-134">String</span><span class="sxs-lookup"><span data-stu-id="2f1ae-134">String</span></span>|<span data-ttu-id="2f1ae-135">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-135">The policy's description.</span></span> <span data-ttu-id="2f1ae-136">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1ae-137">createdDateTime</span></span>|<span data-ttu-id="2f1ae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1ae-138">DateTimeOffset</span></span>|<span data-ttu-id="2f1ae-139">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-139">The date and time the group was created.</span></span> <span data-ttu-id="2f1ae-140">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1ae-141">lastModifiedDateTime</span></span>|<span data-ttu-id="2f1ae-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1ae-142">DateTimeOffset</span></span>|<span data-ttu-id="2f1ae-143">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-143">Last time the policy was modified.</span></span> <span data-ttu-id="2f1ae-144">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-145">id</span><span class="sxs-lookup"><span data-stu-id="2f1ae-145">id</span></span>|<span data-ttu-id="2f1ae-146">String</span><span class="sxs-lookup"><span data-stu-id="2f1ae-146">String</span></span>|<span data-ttu-id="2f1ae-147">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-147">Key of the setting.</span></span> <span data-ttu-id="2f1ae-148">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-149">version</span><span class="sxs-lookup"><span data-stu-id="2f1ae-149">version</span></span>|<span data-ttu-id="2f1ae-150">String</span><span class="sxs-lookup"><span data-stu-id="2f1ae-150">String</span></span>|<span data-ttu-id="2f1ae-151">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-151">Version of the entity.</span></span> <span data-ttu-id="2f1ae-152">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f1ae-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="2f1ae-153">customSettings</span></span>|<span data-ttu-id="2f1ae-154">Коллекция [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2f1ae-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f1ae-155">Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f1ae-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="2f1ae-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="2f1ae-156">deployedAppCount</span></span>|<span data-ttu-id="2f1ae-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1ae-157">Int32</span></span>|<span data-ttu-id="2f1ae-158">Количество приложений, для которых развернута текущая политика.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="2f1ae-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2f1ae-159">isAssigned</span></span>|<span data-ttu-id="2f1ae-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f1ae-160">Boolean</span></span>|<span data-ttu-id="2f1ae-161">Указывает, развернута ли политика для групп включения.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="2f1ae-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f1ae-162">Response</span></span>
<span data-ttu-id="2f1ae-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1ae-164">Пример</span><span class="sxs-lookup"><span data-stu-id="2f1ae-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f1ae-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f1ae-165">Request</span></span>
<span data-ttu-id="2f1ae-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
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

### <a name="response"></a><span data-ttu-id="2f1ae-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f1ae-167">Response</span></span>
<span data-ttu-id="2f1ae-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f1ae-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



