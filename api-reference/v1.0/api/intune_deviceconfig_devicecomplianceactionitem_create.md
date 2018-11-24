# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="e7619-101">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="e7619-101">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="e7619-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7619-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7619-103">Создание объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="e7619-103">Create a new [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7619-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7619-104">Prerequisites</span></span>
<span data-ttu-id="e7619-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7619-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7619-107">Permission type</span></span>|<span data-ttu-id="e7619-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7619-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7619-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7619-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7619-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7619-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7619-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7619-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7619-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7619-112">Not supported.</span></span>|
|<span data-ttu-id="e7619-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7619-113">Application</span></span>|<span data-ttu-id="e7619-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7619-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7619-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7619-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7619-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7619-116">Request headers</span></span>
|<span data-ttu-id="e7619-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7619-117">Header</span></span>|<span data-ttu-id="e7619-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e7619-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7619-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7619-119">Authorization</span></span>|<span data-ttu-id="e7619-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7619-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7619-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7619-121">Accept</span></span>|<span data-ttu-id="e7619-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7619-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7619-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7619-123">Request body</span></span>
<span data-ttu-id="e7619-124">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7619-124">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="e7619-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="e7619-125">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="e7619-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7619-126">Property</span></span>|<span data-ttu-id="e7619-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e7619-127">Type</span></span>|<span data-ttu-id="e7619-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e7619-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7619-129">id</span><span class="sxs-lookup"><span data-stu-id="e7619-129">id</span></span>|<span data-ttu-id="e7619-130">String</span><span class="sxs-lookup"><span data-stu-id="e7619-130">String</span></span>|<span data-ttu-id="e7619-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7619-131">Key of the entity.</span></span>|
|<span data-ttu-id="e7619-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="e7619-132">gracePeriodHours</span></span>|<span data-ttu-id="e7619-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e7619-133">Int32</span></span>|<span data-ttu-id="e7619-134">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="e7619-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="e7619-135">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="e7619-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="e7619-136">actionType</span><span class="sxs-lookup"><span data-stu-id="e7619-136">actionType</span></span>|[<span data-ttu-id="e7619-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="e7619-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="e7619-138">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="e7619-138">What action to take.</span></span> <span data-ttu-id="e7619-139">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="e7619-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="e7619-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="e7619-140">notificationTemplateId</span></span>|<span data-ttu-id="e7619-141">String</span><span class="sxs-lookup"><span data-stu-id="e7619-141">String</span></span>|<span data-ttu-id="e7619-142">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="e7619-142">What notification Message template to use</span></span>|
|<span data-ttu-id="e7619-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="e7619-143">notificationMessageCCList</span></span>|<span data-ttu-id="e7619-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e7619-144">String collection</span></span>|<span data-ttu-id="e7619-145">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="e7619-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="e7619-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7619-146">Response</span></span>
<span data-ttu-id="e7619-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7619-147">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7619-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e7619-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7619-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7619-149">Request</span></span>
<span data-ttu-id="e7619-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7619-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7619-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7619-151">Response</span></span>
<span data-ttu-id="e7619-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e7619-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



