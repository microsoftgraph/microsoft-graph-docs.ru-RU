# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="c26f2-101">Создание iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="c26f2-101">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="c26f2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c26f2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c26f2-103">Создание объекта [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-103">Create a new [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c26f2-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c26f2-104">Prerequisites</span></span>
<span data-ttu-id="c26f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c26f2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c26f2-107">Permission type</span></span>|<span data-ttu-id="c26f2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c26f2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c26f2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c26f2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c26f2-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26f2-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c26f2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c26f2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c26f2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c26f2-112">Not supported.</span></span>|
|<span data-ttu-id="c26f2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c26f2-113">Application</span></span>|<span data-ttu-id="c26f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c26f2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c26f2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c26f2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c26f2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c26f2-116">Request headers</span></span>
|<span data-ttu-id="c26f2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c26f2-117">Header</span></span>|<span data-ttu-id="c26f2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c26f2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c26f2-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c26f2-119">Authorization</span></span>|<span data-ttu-id="c26f2-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c26f2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c26f2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c26f2-121">Accept</span></span>|<span data-ttu-id="c26f2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c26f2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c26f2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c26f2-123">Request body</span></span>
<span data-ttu-id="c26f2-124">В теле запроса добавьте представление объекта iosUpdateConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c26f2-124">In the request body, supply a JSON representation for the iosUpdateConfiguration object.</span></span>

<span data-ttu-id="c26f2-125">Ниже показаны свойства, которые необходимо указывать при создании объекта iosUpdateConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c26f2-125">The following table shows the properties that are required when you create the iosUpdateConfiguration.</span></span>

|<span data-ttu-id="c26f2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c26f2-126">Property</span></span>|<span data-ttu-id="c26f2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c26f2-127">Type</span></span>|<span data-ttu-id="c26f2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c26f2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c26f2-129">id</span><span class="sxs-lookup"><span data-stu-id="c26f2-129">id</span></span>|<span data-ttu-id="c26f2-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c26f2-130">String</span></span>|<span data-ttu-id="c26f2-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c26f2-131">Key of the entity.</span></span> <span data-ttu-id="c26f2-132">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c26f2-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c26f2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c26f2-134">DateTimeOffset</span></span>|<span data-ttu-id="c26f2-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c26f2-135">DateTime the object was last modified.</span></span> <span data-ttu-id="c26f2-136">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c26f2-137">createdDateTime</span></span>|<span data-ttu-id="c26f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c26f2-138">DateTimeOffset</span></span>|<span data-ttu-id="c26f2-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c26f2-139">DateTime the object was created.</span></span> <span data-ttu-id="c26f2-140">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-141">description</span><span class="sxs-lookup"><span data-stu-id="c26f2-141">description</span></span>|<span data-ttu-id="c26f2-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c26f2-142">String</span></span>|<span data-ttu-id="c26f2-143">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c26f2-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c26f2-144">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c26f2-145">displayName</span></span>|<span data-ttu-id="c26f2-146">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c26f2-146">String</span></span>|<span data-ttu-id="c26f2-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c26f2-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c26f2-148">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-149">version</span><span class="sxs-lookup"><span data-stu-id="c26f2-149">version</span></span>|<span data-ttu-id="c26f2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c26f2-150">Int32</span></span>|<span data-ttu-id="c26f2-151">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c26f2-151">Version of the device configuration.</span></span> <span data-ttu-id="c26f2-152">Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c26f2-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c26f2-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="c26f2-153">activeHoursStart</span></span>|<span data-ttu-id="c26f2-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c26f2-154">TimeOfDay</span></span>|<span data-ttu-id="c26f2-155">Начало периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="c26f2-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="c26f2-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="c26f2-156">activeHoursEnd</span></span>|<span data-ttu-id="c26f2-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c26f2-157">TimeOfDay</span></span>|<span data-ttu-id="c26f2-158">Завершение периода активности (период активности — временной промежуток, в течение которого не должны устанавливаться обновления).</span><span class="sxs-lookup"><span data-stu-id="c26f2-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="c26f2-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="c26f2-159">scheduledInstallDays</span></span>|<span data-ttu-id="c26f2-160">Коллекция [перечисления dayOfWeek](../resources/intune_deviceconfig_dayofweek.md)</span><span class="sxs-lookup"><span data-stu-id="c26f2-160">[dayOfWeek enum](../resources/intune_deviceconfig_dayofweek.md) collection</span></span>|<span data-ttu-id="c26f2-161">Дни недели, для которых настраиваются часы активности.</span><span class="sxs-lookup"><span data-stu-id="c26f2-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="c26f2-162">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="c26f2-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="c26f2-163">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="c26f2-163">The possible values are `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , , , or .</span></span>|
|<span data-ttu-id="c26f2-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="c26f2-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="c26f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c26f2-165">Int32</span></span>|<span data-ttu-id="c26f2-166">Сдвиг по времени от UTC (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c26f2-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="c26f2-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="c26f2-167">Response</span></span>
<span data-ttu-id="c26f2-168">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c26f2-168">If successful, this method returns a `201 Created` response code and a [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26f2-169">Пример</span><span class="sxs-lookup"><span data-stu-id="c26f2-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="c26f2-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c26f2-170">Request</span></span>
<span data-ttu-id="c26f2-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c26f2-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="c26f2-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="c26f2-172">Response</span></span>
<span data-ttu-id="c26f2-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c26f2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



