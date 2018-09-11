# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="a2dcc-101">Создание объекта notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a2dcc-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="a2dcc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2dcc-103">Создание объекта [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).</span><span class="sxs-lookup"><span data-stu-id="a2dcc-103">Create a new [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2dcc-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2dcc-104">Prerequisites</span></span>
<span data-ttu-id="a2dcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2dcc-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2dcc-107">Permission type</span></span>|<span data-ttu-id="a2dcc-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2dcc-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2dcc-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2dcc-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a2dcc-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2dcc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-112">Not supported.</span></span>|
|<span data-ttu-id="a2dcc-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2dcc-113">Application</span></span>|<span data-ttu-id="a2dcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2dcc-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2dcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="a2dcc-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2dcc-116">Request headers</span></span>
|<span data-ttu-id="a2dcc-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2dcc-117">Header</span></span>|<span data-ttu-id="a2dcc-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a2dcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2dcc-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2dcc-119">Authorization</span></span>|<span data-ttu-id="a2dcc-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a2dcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2dcc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a2dcc-121">Accept</span></span>|<span data-ttu-id="a2dcc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a2dcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2dcc-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2dcc-123">Request body</span></span>
<span data-ttu-id="a2dcc-124">В теле запроса добавьте представление объекта notificationMessageTemplate в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-124">In the request body, supply a JSON representation for the notificationMessageTemplate object.</span></span>

<span data-ttu-id="a2dcc-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта notificationMessageTemplate.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-125">The following table shows the properties that are required when you create the notificationMessageTemplate.</span></span>

|<span data-ttu-id="a2dcc-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2dcc-126">Property</span></span>|<span data-ttu-id="a2dcc-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a2dcc-127">Type</span></span>|<span data-ttu-id="a2dcc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a2dcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2dcc-129">id</span><span class="sxs-lookup"><span data-stu-id="a2dcc-129">id</span></span>|<span data-ttu-id="a2dcc-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-130">String</span></span>|<span data-ttu-id="a2dcc-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-131">Key of the entity.</span></span>|
|<span data-ttu-id="a2dcc-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2dcc-132">lastModifiedDateTime</span></span>|<span data-ttu-id="a2dcc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2dcc-133">DateTimeOffset</span></span>|<span data-ttu-id="a2dcc-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a2dcc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a2dcc-135">displayName</span></span>|<span data-ttu-id="a2dcc-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-136">String</span></span>|<span data-ttu-id="a2dcc-137">Отображаемое имя для шаблона сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="a2dcc-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="a2dcc-138">defaultLocale</span></span>|<span data-ttu-id="a2dcc-139">String (строка)</span><span class="sxs-lookup"><span data-stu-id="a2dcc-139">String</span></span>|<span data-ttu-id="a2dcc-140">Языковой стандарт по умолчанию, который используется, если запрошенный языковой стандарт недоступен.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="a2dcc-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="a2dcc-141">brandingOptions</span></span>|[<span data-ttu-id="a2dcc-142">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="a2dcc-142">notificationTemplateBrandingOptions</span></span>](../resources/intune_notification_notificationtemplatebrandingoptions.md)|<span data-ttu-id="a2dcc-p102">Параметры фирменной символики шаблона сообщения. Фирменная символика определяется в консоли администрирования Intune. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-p102">The Message Template Branding Options. Branding is defined in the Intune Admin Console. The possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2dcc-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2dcc-146">Response</span></span>
<span data-ttu-id="a2dcc-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-147">If successful, this method returns a `201 Created` response code and a [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2dcc-148">Пример</span><span class="sxs-lookup"><span data-stu-id="a2dcc-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2dcc-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2dcc-149">Request</span></span>
<span data-ttu-id="a2dcc-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="a2dcc-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2dcc-151">Response</span></span>
<span data-ttu-id="a2dcc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2dcc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```








