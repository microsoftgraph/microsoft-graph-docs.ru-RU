# <a name="create-localizednotificationmessage"></a><span data-ttu-id="59307-101">Создание объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="59307-101">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="59307-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59307-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59307-103">Создание объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="59307-103">Create a new [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59307-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="59307-104">Prerequisites</span></span>
<span data-ttu-id="59307-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59307-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59307-107">Permission type</span></span>|<span data-ttu-id="59307-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59307-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59307-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59307-109">Delegated (work or school account)</span></span>|<span data-ttu-id="59307-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59307-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="59307-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59307-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59307-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59307-112">Not supported.</span></span>|
|<span data-ttu-id="59307-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59307-113">Application</span></span>|<span data-ttu-id="59307-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59307-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59307-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59307-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="59307-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59307-116">Request headers</span></span>
|<span data-ttu-id="59307-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59307-117">Header</span></span>|<span data-ttu-id="59307-118">Значение</span><span class="sxs-lookup"><span data-stu-id="59307-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59307-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59307-119">Authorization</span></span>|<span data-ttu-id="59307-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="59307-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59307-121">Принять</span><span class="sxs-lookup"><span data-stu-id="59307-121">Accept</span></span>|<span data-ttu-id="59307-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="59307-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59307-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59307-123">Request body</span></span>
<span data-ttu-id="59307-124">В теле запроса добавьте представление объекта localizedNotificationMessage в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59307-124">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="59307-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта localizedNotificationMessage.</span><span class="sxs-lookup"><span data-stu-id="59307-125">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="59307-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="59307-126">Property</span></span>|<span data-ttu-id="59307-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59307-127">Type</span></span>|<span data-ttu-id="59307-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59307-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59307-129">ИД</span><span class="sxs-lookup"><span data-stu-id="59307-129">id</span></span>|<span data-ttu-id="59307-130">Строка</span><span class="sxs-lookup"><span data-stu-id="59307-130">String</span></span>|<span data-ttu-id="59307-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59307-131">Key of the entity.</span></span>|
|<span data-ttu-id="59307-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59307-132">lastModifiedDateTime</span></span>|<span data-ttu-id="59307-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59307-133">DateTimeOffset</span></span>|<span data-ttu-id="59307-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="59307-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="59307-135">языковой стандарт</span><span class="sxs-lookup"><span data-stu-id="59307-135">locale</span></span>|<span data-ttu-id="59307-136">Строка</span><span class="sxs-lookup"><span data-stu-id="59307-136">String</span></span>|<span data-ttu-id="59307-137">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="59307-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="59307-138">тема</span><span class="sxs-lookup"><span data-stu-id="59307-138">subject</span></span>|<span data-ttu-id="59307-139">Строка</span><span class="sxs-lookup"><span data-stu-id="59307-139">String</span></span>|<span data-ttu-id="59307-140">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="59307-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="59307-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="59307-141">messageTemplate</span></span>|<span data-ttu-id="59307-142">Строка</span><span class="sxs-lookup"><span data-stu-id="59307-142">String</span></span>|<span data-ttu-id="59307-143">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="59307-143">The Message Template content.</span></span>|
|<span data-ttu-id="59307-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="59307-144">isDefault</span></span>|<span data-ttu-id="59307-145">Логическое</span><span class="sxs-lookup"><span data-stu-id="59307-145">Boolean</span></span>|<span data-ttu-id="59307-146">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="59307-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="59307-147">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="59307-147">This flag can only be set.</span></span> <span data-ttu-id="59307-148">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="59307-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="59307-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="59307-149">Response</span></span>
<span data-ttu-id="59307-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59307-150">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59307-151">Пример</span><span class="sxs-lookup"><span data-stu-id="59307-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="59307-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="59307-152">Request</span></span>
<span data-ttu-id="59307-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59307-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="59307-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="59307-154">Response</span></span>
<span data-ttu-id="59307-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59307-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```








