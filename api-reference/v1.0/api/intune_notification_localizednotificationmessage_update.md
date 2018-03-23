# <a name="update-localizednotificationmessage"></a><span data-ttu-id="2e295-101">Обновление объекта localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="2e295-101">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="2e295-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e295-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e295-103">Обновление свойств объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="2e295-103">Update the properties of a [calendar](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e295-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e295-104">Prerequisites</span></span>
<span data-ttu-id="2e295-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e295-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e295-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e295-107">Permission type</span></span>|<span data-ttu-id="2e295-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e295-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e295-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e295-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2e295-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e295-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e295-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e295-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e295-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e295-112">Not supported.</span></span>|
|<span data-ttu-id="2e295-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e295-113">Application</span></span>|<span data-ttu-id="2e295-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e295-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e295-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e295-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="2e295-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e295-116">Request headers</span></span>
|<span data-ttu-id="2e295-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e295-117">Header</span></span>|<span data-ttu-id="2e295-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2e295-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e295-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e295-119">Authorization</span></span>|<span data-ttu-id="2e295-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e295-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2e295-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2e295-121">Accept</span></span>|<span data-ttu-id="2e295-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2e295-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e295-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e295-123">Request body</span></span>
<span data-ttu-id="2e295-124">В теле запроса добавьте представление объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e295-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="2e295-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).</span><span class="sxs-lookup"><span data-stu-id="2e295-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2e295-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e295-126">Property</span></span>|<span data-ttu-id="2e295-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2e295-127">Type</span></span>|<span data-ttu-id="2e295-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2e295-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e295-129">id</span><span class="sxs-lookup"><span data-stu-id="2e295-129">id</span></span>|<span data-ttu-id="2e295-130">String</span><span class="sxs-lookup"><span data-stu-id="2e295-130">String</span></span>|<span data-ttu-id="2e295-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2e295-131">Key of the setting.</span></span>|
|<span data-ttu-id="2e295-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e295-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2e295-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e295-133">DateTimeOffset</span></span>|<span data-ttu-id="2e295-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2e295-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2e295-135">locale</span><span class="sxs-lookup"><span data-stu-id="2e295-135">locale</span></span>|<span data-ttu-id="2e295-136">String</span><span class="sxs-lookup"><span data-stu-id="2e295-136">String</span></span>|<span data-ttu-id="2e295-137">Языковой стандарт, для которого предназначено сообщение.</span><span class="sxs-lookup"><span data-stu-id="2e295-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="2e295-138">subject</span><span class="sxs-lookup"><span data-stu-id="2e295-138">subject</span></span>|<span data-ttu-id="2e295-139">String</span><span class="sxs-lookup"><span data-stu-id="2e295-139">String</span></span>|<span data-ttu-id="2e295-140">Тема шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="2e295-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="2e295-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="2e295-141">messageTemplate</span></span>|<span data-ttu-id="2e295-142">String</span><span class="sxs-lookup"><span data-stu-id="2e295-142">String</span></span>|<span data-ttu-id="2e295-143">Содержимое шаблона сообщения.</span><span class="sxs-lookup"><span data-stu-id="2e295-143">The Message Template content.</span></span>|
|<span data-ttu-id="2e295-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="2e295-144">isDefault</span></span>|<span data-ttu-id="2e295-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e295-145">Boolean</span></span>|<span data-ttu-id="2e295-146">Флаг, указывающий, используется ли этот языковой стандарт в качестве базового языка.</span><span class="sxs-lookup"><span data-stu-id="2e295-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="2e295-147">Можно устанавливать только этот флаг.</span><span class="sxs-lookup"><span data-stu-id="2e295-147">This flag can only be set.</span></span> <span data-ttu-id="2e295-148">Чтобы снять его, задайте этому свойству значение true для другого локализованного сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="2e295-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="2e295-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e295-149">Response</span></span>
<span data-ttu-id="2e295-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e295-150">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e295-151">Пример</span><span class="sxs-lookup"><span data-stu-id="2e295-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e295-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e295-152">Request</span></span>
<span data-ttu-id="2e295-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e295-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="2e295-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e295-154">Response</span></span>
<span data-ttu-id="2e295-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e295-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



