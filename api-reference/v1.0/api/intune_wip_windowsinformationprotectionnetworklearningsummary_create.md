# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="2ebd2-101">Создание объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="2ebd2-101">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="2ebd2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ebd2-103">Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2ebd2-103">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ebd2-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ebd2-104">Prerequisites</span></span>
<span data-ttu-id="2ebd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2ebd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ebd2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ebd2-107">Permission type</span></span>|<span data-ttu-id="2ebd2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ebd2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ebd2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ebd2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2ebd2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ebd2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ebd2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ebd2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ebd2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-112">Not supported.</span></span>|
|<span data-ttu-id="2ebd2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ebd2-113">Application</span></span>|<span data-ttu-id="2ebd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ebd2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ebd2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2ebd2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ebd2-116">Request headers</span></span>
|<span data-ttu-id="2ebd2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ebd2-117">Header</span></span>|<span data-ttu-id="2ebd2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2ebd2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ebd2-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ebd2-119">Authorization</span></span>|<span data-ttu-id="2ebd2-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="2ebd2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ebd2-121">Принять</span><span class="sxs-lookup"><span data-stu-id="2ebd2-121">Accept</span></span>|<span data-ttu-id="2ebd2-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="2ebd2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ebd2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ebd2-123">Request body</span></span>
<span data-ttu-id="2ebd2-124">В теле запроса добавьте представление объекта windowsInformationProtectionNetworkLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-124">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="2ebd2-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-125">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="2ebd2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ebd2-126">Property</span></span>|<span data-ttu-id="2ebd2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2ebd2-127">Type</span></span>|<span data-ttu-id="2ebd2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2ebd2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ebd2-129">ИД</span><span class="sxs-lookup"><span data-stu-id="2ebd2-129">id</span></span>|<span data-ttu-id="2ebd2-130">Строка</span><span class="sxs-lookup"><span data-stu-id="2ebd2-130">String</span></span>|<span data-ttu-id="2ebd2-131">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="2ebd2-132">url</span><span class="sxs-lookup"><span data-stu-id="2ebd2-132">url</span></span>|<span data-ttu-id="2ebd2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2ebd2-133">String</span></span>|<span data-ttu-id="2ebd2-134">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="2ebd2-134">Website url</span></span>|
|<span data-ttu-id="2ebd2-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2ebd2-135">deviceCount</span></span>|<span data-ttu-id="2ebd2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2ebd2-136">Int32</span></span>|<span data-ttu-id="2ebd2-137">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="2ebd2-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="2ebd2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ebd2-138">Response</span></span>
<span data-ttu-id="2ebd2-139">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-139">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ebd2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2ebd2-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ebd2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ebd2-141">Request</span></span>
<span data-ttu-id="2ebd2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2ebd2-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ebd2-143">Response</span></span>
<span data-ttu-id="2ebd2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ebd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```








