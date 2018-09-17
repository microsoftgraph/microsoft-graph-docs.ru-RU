# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="efaa0-101">Обновление deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="efaa0-101">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="efaa0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="efaa0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efaa0-103">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="efaa0-103">Update the properties of a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="efaa0-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="efaa0-104">Prerequisites</span></span>
<span data-ttu-id="efaa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="efaa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="efaa0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efaa0-107">Permission type</span></span>|<span data-ttu-id="efaa0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efaa0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efaa0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efaa0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="efaa0-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efaa0-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="efaa0-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efaa0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efaa0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efaa0-112">Not supported.</span></span>|
|<span data-ttu-id="efaa0-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efaa0-113">Application</span></span>|<span data-ttu-id="efaa0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efaa0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="efaa0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efaa0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="efaa0-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efaa0-116">Request headers</span></span>
|<span data-ttu-id="efaa0-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efaa0-117">Header</span></span>|<span data-ttu-id="efaa0-118">Значение</span><span class="sxs-lookup"><span data-stu-id="efaa0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efaa0-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efaa0-119">Authorization</span></span>|<span data-ttu-id="efaa0-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="efaa0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efaa0-121">Принять</span><span class="sxs-lookup"><span data-stu-id="efaa0-121">Accept</span></span>|<span data-ttu-id="efaa0-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="efaa0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efaa0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efaa0-123">Request body</span></span>
<span data-ttu-id="efaa0-124">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efaa0-124">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="efaa0-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="efaa0-125">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="efaa0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="efaa0-126">Property</span></span>|<span data-ttu-id="efaa0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="efaa0-127">Type</span></span>|<span data-ttu-id="efaa0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="efaa0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efaa0-129">ИД</span><span class="sxs-lookup"><span data-stu-id="efaa0-129">id</span></span>|<span data-ttu-id="efaa0-130">Строка</span><span class="sxs-lookup"><span data-stu-id="efaa0-130">String</span></span>|<span data-ttu-id="efaa0-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="efaa0-131">Key of the entity.</span></span>|
|<span data-ttu-id="efaa0-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="efaa0-132">gracePeriodHours</span></span>|<span data-ttu-id="efaa0-133">Int32</span><span class="sxs-lookup"><span data-stu-id="efaa0-133">Int32</span></span>|<span data-ttu-id="efaa0-134">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="efaa0-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="efaa0-135">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="efaa0-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="efaa0-136">actionType</span><span class="sxs-lookup"><span data-stu-id="efaa0-136">actionType</span></span>|[<span data-ttu-id="efaa0-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="efaa0-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="efaa0-138">Какое действие предпринять.</span><span class="sxs-lookup"><span data-stu-id="efaa0-138">What action to take Possible values are: , , , , , .</span></span> <span data-ttu-id="efaa0-139">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="efaa0-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="efaa0-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="efaa0-140">notificationTemplateId</span></span>|<span data-ttu-id="efaa0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="efaa0-141">String</span></span>|<span data-ttu-id="efaa0-142">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="efaa0-142">What notification Message template to use</span></span>|
|<span data-ttu-id="efaa0-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="efaa0-143">notificationMessageCCList</span></span>|<span data-ttu-id="efaa0-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="efaa0-144">String collection</span></span>|<span data-ttu-id="efaa0-145">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="efaa0-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="efaa0-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="efaa0-146">Response</span></span>
<span data-ttu-id="efaa0-147">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="efaa0-147">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efaa0-148">Пример</span><span class="sxs-lookup"><span data-stu-id="efaa0-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="efaa0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="efaa0-149">Request</span></span>
<span data-ttu-id="efaa0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efaa0-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="efaa0-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="efaa0-151">Response</span></span>
<span data-ttu-id="efaa0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efaa0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








