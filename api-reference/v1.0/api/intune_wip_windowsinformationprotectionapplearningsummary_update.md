# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="43340-101">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="43340-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="43340-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43340-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43340-103">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="43340-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43340-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="43340-104">Prerequisites</span></span>
<span data-ttu-id="43340-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="43340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="43340-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43340-107">Permission type</span></span>|<span data-ttu-id="43340-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43340-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43340-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43340-109">Delegated (work or school account)</span></span>|<span data-ttu-id="43340-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43340-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43340-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43340-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43340-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43340-112">Not supported.</span></span>|
|<span data-ttu-id="43340-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43340-113">Application</span></span>|<span data-ttu-id="43340-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43340-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43340-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43340-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="43340-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43340-116">Request headers</span></span>
|<span data-ttu-id="43340-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43340-117">Header</span></span>|<span data-ttu-id="43340-118">Значение</span><span class="sxs-lookup"><span data-stu-id="43340-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43340-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43340-119">Authorization</span></span>|<span data-ttu-id="43340-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="43340-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43340-121">Accept</span><span class="sxs-lookup"><span data-stu-id="43340-121">Accept</span></span>|<span data-ttu-id="43340-122">application/json</span><span class="sxs-lookup"><span data-stu-id="43340-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43340-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43340-123">Request body</span></span>
<span data-ttu-id="43340-124">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43340-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="43340-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="43340-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="43340-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="43340-126">Property</span></span>|<span data-ttu-id="43340-127">Тип</span><span class="sxs-lookup"><span data-stu-id="43340-127">Type</span></span>|<span data-ttu-id="43340-128">Описание</span><span class="sxs-lookup"><span data-stu-id="43340-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43340-129">id</span><span class="sxs-lookup"><span data-stu-id="43340-129">id</span></span>|<span data-ttu-id="43340-130">Строка</span><span class="sxs-lookup"><span data-stu-id="43340-130">String</span></span>|<span data-ttu-id="43340-131">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="43340-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="43340-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="43340-132">applicationName</span></span>|<span data-ttu-id="43340-133">Строка</span><span class="sxs-lookup"><span data-stu-id="43340-133">String</span></span>|<span data-ttu-id="43340-134">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="43340-134">Application Name</span></span>|
|<span data-ttu-id="43340-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="43340-135">applicationType</span></span>|[<span data-ttu-id="43340-136">applicationType</span><span class="sxs-lookup"><span data-stu-id="43340-136">applicationType</span></span>](../resources/intune_wip_applicationtype.md)|<span data-ttu-id="43340-137">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="43340-137">Target Application Type</span></span> <span data-ttu-id="43340-138">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="43340-138">The possible values are:</span></span>|
|<span data-ttu-id="43340-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="43340-139">deviceCount</span></span>|<span data-ttu-id="43340-140">Int32</span><span class="sxs-lookup"><span data-stu-id="43340-140">Int32</span></span>|<span data-ttu-id="43340-141">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="43340-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="43340-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="43340-142">Response</span></span>
<span data-ttu-id="43340-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="43340-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43340-144">Пример</span><span class="sxs-lookup"><span data-stu-id="43340-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="43340-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="43340-145">Request</span></span>
<span data-ttu-id="43340-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43340-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 106

{
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="43340-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="43340-147">Response</span></span>
<span data-ttu-id="43340-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43340-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



