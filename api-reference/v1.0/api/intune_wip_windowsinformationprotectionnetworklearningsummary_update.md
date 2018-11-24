# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="07466-101">Обновление объекта windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="07466-101">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="07466-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07466-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07466-103">Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="07466-103">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07466-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="07466-104">Prerequisites</span></span>
<span data-ttu-id="07466-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="07466-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="07466-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07466-107">Permission type</span></span>|<span data-ttu-id="07466-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07466-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07466-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07466-109">Delegated (work or school account)</span></span>|<span data-ttu-id="07466-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07466-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07466-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07466-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07466-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07466-112">Not supported.</span></span>|
|<span data-ttu-id="07466-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07466-113">Application</span></span>|<span data-ttu-id="07466-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07466-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07466-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07466-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="07466-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07466-116">Request headers</span></span>
|<span data-ttu-id="07466-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07466-117">Header</span></span>|<span data-ttu-id="07466-118">Значение</span><span class="sxs-lookup"><span data-stu-id="07466-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07466-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="07466-119">Authorization</span></span>|<span data-ttu-id="07466-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07466-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07466-121">Accept</span><span class="sxs-lookup"><span data-stu-id="07466-121">Accept</span></span>|<span data-ttu-id="07466-122">application/json</span><span class="sxs-lookup"><span data-stu-id="07466-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07466-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07466-123">Request body</span></span>
<span data-ttu-id="07466-124">В теле запроса добавьте представление объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07466-124">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="07466-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="07466-125">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="07466-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="07466-126">Property</span></span>|<span data-ttu-id="07466-127">Тип</span><span class="sxs-lookup"><span data-stu-id="07466-127">Type</span></span>|<span data-ttu-id="07466-128">Описание</span><span class="sxs-lookup"><span data-stu-id="07466-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07466-129">id</span><span class="sxs-lookup"><span data-stu-id="07466-129">id</span></span>|<span data-ttu-id="07466-130">String</span><span class="sxs-lookup"><span data-stu-id="07466-130">String</span></span>|<span data-ttu-id="07466-131">Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="07466-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="07466-132">url</span><span class="sxs-lookup"><span data-stu-id="07466-132">url</span></span>|<span data-ttu-id="07466-133">String</span><span class="sxs-lookup"><span data-stu-id="07466-133">String</span></span>|<span data-ttu-id="07466-134">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="07466-134">Website url</span></span>|
|<span data-ttu-id="07466-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="07466-135">deviceCount</span></span>|<span data-ttu-id="07466-136">Int32</span><span class="sxs-lookup"><span data-stu-id="07466-136">Int32</span></span>|<span data-ttu-id="07466-137">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="07466-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="07466-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="07466-138">Response</span></span>
<span data-ttu-id="07466-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="07466-139">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07466-140">Пример</span><span class="sxs-lookup"><span data-stu-id="07466-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="07466-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="07466-141">Request</span></span>
<span data-ttu-id="07466-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07466-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="07466-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="07466-143">Response</span></span>
<span data-ttu-id="07466-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07466-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



