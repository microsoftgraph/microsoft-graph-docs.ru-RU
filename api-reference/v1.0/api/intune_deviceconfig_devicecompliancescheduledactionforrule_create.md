# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="11827-101">Создание объекта deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="11827-101">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="11827-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11827-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11827-103">Создание объекта [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="11827-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11827-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11827-104">Prerequisites</span></span>
<span data-ttu-id="11827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11827-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11827-107">Permission type</span></span>|<span data-ttu-id="11827-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11827-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11827-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11827-109">Delegated (work or school account)</span></span>|<span data-ttu-id="11827-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11827-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11827-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11827-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11827-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11827-112">Not supported.</span></span>|
|<span data-ttu-id="11827-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11827-113">Application</span></span>|<span data-ttu-id="11827-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11827-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11827-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11827-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="11827-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11827-116">Request headers</span></span>
|<span data-ttu-id="11827-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11827-117">Header</span></span>|<span data-ttu-id="11827-118">Значение</span><span class="sxs-lookup"><span data-stu-id="11827-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11827-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="11827-119">Authorization</span></span>|<span data-ttu-id="11827-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11827-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="11827-121">Accept</span><span class="sxs-lookup"><span data-stu-id="11827-121">Accept</span></span>|<span data-ttu-id="11827-122">application/json</span><span class="sxs-lookup"><span data-stu-id="11827-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11827-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11827-123">Request body</span></span>
<span data-ttu-id="11827-124">В теле запроса добавьте представление объекта deviceComplianceScheduledActionForRule в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11827-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="11827-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceComplianceScheduledActionForRule.</span><span class="sxs-lookup"><span data-stu-id="11827-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="11827-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="11827-126">Property</span></span>|<span data-ttu-id="11827-127">Тип</span><span class="sxs-lookup"><span data-stu-id="11827-127">Type</span></span>|<span data-ttu-id="11827-128">Описание</span><span class="sxs-lookup"><span data-stu-id="11827-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11827-129">id</span><span class="sxs-lookup"><span data-stu-id="11827-129">id</span></span>|<span data-ttu-id="11827-130">String</span><span class="sxs-lookup"><span data-stu-id="11827-130">String</span></span>|<span data-ttu-id="11827-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11827-131">Key of the setting.</span></span>|
|<span data-ttu-id="11827-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="11827-132">ruleName</span></span>|<span data-ttu-id="11827-133">String</span><span class="sxs-lookup"><span data-stu-id="11827-133">String</span></span>|<span data-ttu-id="11827-134">Имя правила, к которому применяется это запланированное действие.</span><span class="sxs-lookup"><span data-stu-id="11827-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="11827-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="11827-135">Response</span></span>
<span data-ttu-id="11827-136">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11827-136">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11827-137">Пример</span><span class="sxs-lookup"><span data-stu-id="11827-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="11827-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="11827-138">Request</span></span>
<span data-ttu-id="11827-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11827-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="11827-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="11827-140">Response</span></span>
<span data-ttu-id="11827-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="11827-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



