# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="75d27-101">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="75d27-101">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="75d27-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="75d27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75d27-103">Создание объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="75d27-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75d27-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75d27-104">Prerequisites</span></span>
<span data-ttu-id="75d27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="75d27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75d27-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75d27-107">Permission type</span></span>|<span data-ttu-id="75d27-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75d27-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75d27-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75d27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="75d27-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75d27-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75d27-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75d27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75d27-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75d27-112">Not supported.</span></span>|
|<span data-ttu-id="75d27-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75d27-113">Application</span></span>|<span data-ttu-id="75d27-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75d27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75d27-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75d27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75d27-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75d27-116">Request headers</span></span>
|<span data-ttu-id="75d27-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75d27-117">Header</span></span>|<span data-ttu-id="75d27-118">Значение</span><span class="sxs-lookup"><span data-stu-id="75d27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75d27-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="75d27-119">Authorization</span></span>|<span data-ttu-id="75d27-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75d27-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75d27-121">Accept</span><span class="sxs-lookup"><span data-stu-id="75d27-121">Accept</span></span>|<span data-ttu-id="75d27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="75d27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75d27-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75d27-123">Request body</span></span>
<span data-ttu-id="75d27-124">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75d27-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="75d27-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="75d27-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="75d27-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="75d27-126">Property</span></span>|<span data-ttu-id="75d27-127">Тип</span><span class="sxs-lookup"><span data-stu-id="75d27-127">Type</span></span>|<span data-ttu-id="75d27-128">Описание</span><span class="sxs-lookup"><span data-stu-id="75d27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75d27-129">id</span><span class="sxs-lookup"><span data-stu-id="75d27-129">id</span></span>|<span data-ttu-id="75d27-130">String</span><span class="sxs-lookup"><span data-stu-id="75d27-130">String</span></span>|<span data-ttu-id="75d27-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75d27-131">Key of the setting.</span></span>|
|<span data-ttu-id="75d27-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="75d27-132">gracePeriodHours</span></span>|<span data-ttu-id="75d27-133">Int32</span><span class="sxs-lookup"><span data-stu-id="75d27-133">Int32</span></span>|<span data-ttu-id="75d27-134">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="75d27-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="75d27-135">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="75d27-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="75d27-136">actionType</span><span class="sxs-lookup"><span data-stu-id="75d27-136">actionType</span></span>|<span data-ttu-id="75d27-137">String</span><span class="sxs-lookup"><span data-stu-id="75d27-137">String</span></span>|<span data-ttu-id="75d27-138">Выполняемое действие. Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span><span class="sxs-lookup"><span data-stu-id="75d27-138">What action to take Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span></span>|
|<span data-ttu-id="75d27-139">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="75d27-139">notificationTemplateId</span></span>|<span data-ttu-id="75d27-140">String</span><span class="sxs-lookup"><span data-stu-id="75d27-140">String</span></span>|<span data-ttu-id="75d27-141">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="75d27-141">What notification Message template to use</span></span>|
|<span data-ttu-id="75d27-142">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="75d27-142">notificationMessageCCList</span></span>|<span data-ttu-id="75d27-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="75d27-143">String collection</span></span>|<span data-ttu-id="75d27-144">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="75d27-144">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="75d27-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="75d27-145">Response</span></span>
<span data-ttu-id="75d27-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75d27-146">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75d27-147">Пример</span><span class="sxs-lookup"><span data-stu-id="75d27-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="75d27-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="75d27-148">Request</span></span>
<span data-ttu-id="75d27-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75d27-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="75d27-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="75d27-150">Response</span></span>
<span data-ttu-id="75d27-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75d27-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```



