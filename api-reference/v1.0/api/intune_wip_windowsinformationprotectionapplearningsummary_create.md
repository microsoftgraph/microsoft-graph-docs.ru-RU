# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="2d32f-101">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2d32f-101">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="2d32f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d32f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d32f-103">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2d32f-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d32f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2d32f-104">Prerequisites</span></span>
<span data-ttu-id="2d32f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2d32f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d32f-107">Permission type</span></span>|<span data-ttu-id="2d32f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d32f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d32f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d32f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2d32f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d32f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d32f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d32f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d32f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d32f-112">Not supported.</span></span>|
|<span data-ttu-id="2d32f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d32f-113">Application</span></span>|<span data-ttu-id="2d32f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d32f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d32f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d32f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2d32f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d32f-116">Request headers</span></span>
|<span data-ttu-id="2d32f-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d32f-117">Header</span></span>|<span data-ttu-id="2d32f-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2d32f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d32f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d32f-119">Authorization</span></span>|<span data-ttu-id="2d32f-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d32f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d32f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2d32f-121">Accept</span></span>|<span data-ttu-id="2d32f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2d32f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d32f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d32f-123">Request body</span></span>
<span data-ttu-id="2d32f-124">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d32f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="2d32f-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2d32f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2d32f-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d32f-126">Property</span></span>|<span data-ttu-id="2d32f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2d32f-127">Type</span></span>|<span data-ttu-id="2d32f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2d32f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d32f-129">id</span><span class="sxs-lookup"><span data-stu-id="2d32f-129">id</span></span>|<span data-ttu-id="2d32f-130">String</span><span class="sxs-lookup"><span data-stu-id="2d32f-130">String</span></span>|<span data-ttu-id="2d32f-131">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2d32f-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="2d32f-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="2d32f-132">applicationName</span></span>|<span data-ttu-id="2d32f-133">String</span><span class="sxs-lookup"><span data-stu-id="2d32f-133">String</span></span>|<span data-ttu-id="2d32f-134">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="2d32f-134">Application Name</span></span>|
|<span data-ttu-id="2d32f-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="2d32f-135">applicationType</span></span>|<span data-ttu-id="2d32f-136">String</span><span class="sxs-lookup"><span data-stu-id="2d32f-136">String</span></span>|<span data-ttu-id="2d32f-137">Тип приложения. Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="2d32f-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="2d32f-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2d32f-138">deviceCount</span></span>|<span data-ttu-id="2d32f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2d32f-139">Int32</span></span>|<span data-ttu-id="2d32f-140">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="2d32f-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2d32f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d32f-141">Response</span></span>
<span data-ttu-id="2d32f-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d32f-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d32f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2d32f-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d32f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d32f-144">Request</span></span>
<span data-ttu-id="2d32f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d32f-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2d32f-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d32f-146">Response</span></span>
<span data-ttu-id="2d32f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2d32f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



