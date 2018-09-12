# <a name="update-auditevent"></a><span data-ttu-id="7fb1c-101">Обновление объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="7fb1c-101">Update auditEvent</span></span>

> <span data-ttu-id="7fb1c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fb1c-103">Обновление свойств объекта [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fb1c-103">Update the properties of a [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fb1c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb1c-104">Prerequisites</span></span>
<span data-ttu-id="7fb1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7fb1c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fb1c-107">Permission type</span></span>|<span data-ttu-id="7fb1c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fb1c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7fb1c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fb1c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7fb1c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fb1c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-112">Not supported.</span></span>|
|<span data-ttu-id="7fb1c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fb1c-113">Application</span></span>|<span data-ttu-id="7fb1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fb1c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fb1c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="7fb1c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fb1c-116">Request headers</span></span>
|<span data-ttu-id="7fb1c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fb1c-117">Header</span></span>|<span data-ttu-id="7fb1c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7fb1c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fb1c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fb1c-119">Authorization</span></span>|<span data-ttu-id="7fb1c-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="7fb1c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fb1c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7fb1c-121">Accept</span></span>|<span data-ttu-id="7fb1c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7fb1c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fb1c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fb1c-123">Request body</span></span>
<span data-ttu-id="7fb1c-124">В теле запроса добавьте представление объекта [auditEvent](../resources/intune_auditing_auditevent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-124">In the request body, supply a JSON representation for the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>

<span data-ttu-id="7fb1c-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [auditEvent](../resources/intune_auditing_auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="7fb1c-125">The following table shows the properties that are required when you create the [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>

|<span data-ttu-id="7fb1c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fb1c-126">Property</span></span>|<span data-ttu-id="7fb1c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7fb1c-127">Type</span></span>|<span data-ttu-id="7fb1c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7fb1c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fb1c-129">id</span><span class="sxs-lookup"><span data-stu-id="7fb1c-129">id</span></span>|<span data-ttu-id="7fb1c-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-130">String</span></span>|<span data-ttu-id="7fb1c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-131">Key of the entity.</span></span>|
|<span data-ttu-id="7fb1c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7fb1c-132">displayName</span></span>|<span data-ttu-id="7fb1c-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-133">String</span></span>|<span data-ttu-id="7fb1c-134">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-134">Event display name.</span></span>|
|<span data-ttu-id="7fb1c-135">componentName</span><span class="sxs-lookup"><span data-stu-id="7fb1c-135">componentName</span></span>|<span data-ttu-id="7fb1c-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-136">String</span></span>|<span data-ttu-id="7fb1c-137">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-137">Component name.</span></span>|
|<span data-ttu-id="7fb1c-138">actor</span><span class="sxs-lookup"><span data-stu-id="7fb1c-138">actor</span></span>|[<span data-ttu-id="7fb1c-139">auditActor</span><span class="sxs-lookup"><span data-stu-id="7fb1c-139">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="7fb1c-140">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-140">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="7fb1c-141">activity</span><span class="sxs-lookup"><span data-stu-id="7fb1c-141">activity</span></span>|<span data-ttu-id="7fb1c-142">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-142">String</span></span>|<span data-ttu-id="7fb1c-143">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-143">Friendly name of the activity.</span></span>|
|<span data-ttu-id="7fb1c-144">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="7fb1c-144">activityDateTime</span></span>|<span data-ttu-id="7fb1c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fb1c-145">DateTimeOffset</span></span>|<span data-ttu-id="7fb1c-146">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="7fb1c-146">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="7fb1c-147">activityType</span><span class="sxs-lookup"><span data-stu-id="7fb1c-147">activityType</span></span>|<span data-ttu-id="7fb1c-148">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-148">String</span></span>|<span data-ttu-id="7fb1c-149">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-149">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="7fb1c-150">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="7fb1c-150">activityOperationType</span></span>|<span data-ttu-id="7fb1c-151">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-151">String</span></span>|<span data-ttu-id="7fb1c-152">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-152">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="7fb1c-153">activityResult</span><span class="sxs-lookup"><span data-stu-id="7fb1c-153">activityResult</span></span>|<span data-ttu-id="7fb1c-154">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-154">String</span></span>|<span data-ttu-id="7fb1c-155">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-155">The result of the activity.</span></span>|
|<span data-ttu-id="7fb1c-156">correlationId</span><span class="sxs-lookup"><span data-stu-id="7fb1c-156">correlationId</span></span>|<span data-ttu-id="7fb1c-157">Guid</span><span class="sxs-lookup"><span data-stu-id="7fb1c-157">Guid</span></span>|<span data-ttu-id="7fb1c-158">Идентификатор клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-158">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="7fb1c-159">resources</span><span class="sxs-lookup"><span data-stu-id="7fb1c-159">resources</span></span>|<span data-ttu-id="7fb1c-160">Коллекция [auditResource](../resources/intune_auditing_auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-160">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="7fb1c-161">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-161">Resources being modified.</span></span>|
|<span data-ttu-id="7fb1c-162">category</span><span class="sxs-lookup"><span data-stu-id="7fb1c-162">category</span></span>|<span data-ttu-id="7fb1c-163">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7fb1c-163">String</span></span>|<span data-ttu-id="7fb1c-164">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-164">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="7fb1c-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb1c-165">Response</span></span>
<span data-ttu-id="7fb1c-166">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [auditEvent](../resources/intune_auditing_auditevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-166">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fb1c-167">Пример</span><span class="sxs-lookup"><span data-stu-id="7fb1c-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fb1c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fb1c-168">Request</span></span>
<span data-ttu-id="7fb1c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1338

{
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="7fb1c-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fb1c-170">Response</span></span>
<span data-ttu-id="7fb1c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fb1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```








