# <a name="update-devicemanagement"></a><span data-ttu-id="eb114-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="eb114-101">Update deviceManagement</span></span>

> <span data-ttu-id="eb114-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eb114-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb114-103">Обновление свойств объекта [deviceManagement](../resources/intune_onboarding_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="eb114-103">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb114-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eb114-104">Prerequisites</span></span>
<span data-ttu-id="eb114-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb114-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb114-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb114-107">Permission type</span></span>|<span data-ttu-id="eb114-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb114-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb114-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb114-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eb114-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb114-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb114-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb114-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb114-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb114-112">Not supported.</span></span>|
|<span data-ttu-id="eb114-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb114-113">Application</span></span>|<span data-ttu-id="eb114-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb114-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb114-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb114-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="eb114-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb114-116">Request headers</span></span>
|<span data-ttu-id="eb114-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb114-117">Header</span></span>|<span data-ttu-id="eb114-118">Значение</span><span class="sxs-lookup"><span data-stu-id="eb114-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb114-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb114-119">Authorization</span></span>|<span data-ttu-id="eb114-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb114-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eb114-121">Accept</span><span class="sxs-lookup"><span data-stu-id="eb114-121">Accept</span></span>|<span data-ttu-id="eb114-122">application/json</span><span class="sxs-lookup"><span data-stu-id="eb114-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb114-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb114-123">Request body</span></span>
<span data-ttu-id="eb114-124">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_onboarding_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb114-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_devicemanagement.md) object.</span></span>

<span data-ttu-id="eb114-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_onboarding_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="eb114-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="eb114-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb114-126">Property</span></span>|<span data-ttu-id="eb114-127">Тип</span><span class="sxs-lookup"><span data-stu-id="eb114-127">Type</span></span>|<span data-ttu-id="eb114-128">Описание</span><span class="sxs-lookup"><span data-stu-id="eb114-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb114-129">id</span><span class="sxs-lookup"><span data-stu-id="eb114-129">id</span></span>|<span data-ttu-id="eb114-130">String</span><span class="sxs-lookup"><span data-stu-id="eb114-130">String</span></span>|<span data-ttu-id="eb114-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb114-131">Not yet documented</span></span>|
|<span data-ttu-id="eb114-132">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="eb114-132">intuneBrand</span></span>|[<span data-ttu-id="eb114-133">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="eb114-133">intuneBrand</span></span>](../resources/intune_onboarding_intunebrand.md)|<span data-ttu-id="eb114-134">Ресурс intuneBrand содержит данные, которые используются для настройки внешнего вида приложения "Корпоративный портал" и веб-портала пользователя.</span><span class="sxs-lookup"><span data-stu-id="eb114-134">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|



## <a name="response"></a><span data-ttu-id="eb114-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb114-135">Response</span></span>
<span data-ttu-id="eb114-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_onboarding_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb114-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb114-137">Пример</span><span class="sxs-lookup"><span data-stu-id="eb114-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb114-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb114-138">Request</span></span>
<span data-ttu-id="eb114-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb114-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 1043

{
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```

### <a name="response"></a><span data-ttu-id="eb114-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb114-140">Response</span></span>
<span data-ttu-id="eb114-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eb114-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1147

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "intuneBrand": {
    "@odata.type": "microsoft.graph.intuneBrand",
    "displayName": "Display Name value",
    "contactITName": "Contact ITName value",
    "contactITPhoneNumber": "Contact ITPhone Number value",
    "contactITEmailAddress": "Contact ITEmail Address value",
    "contactITNotes": "Contact ITNotes value",
    "privacyUrl": "https://example.com/privacyUrl/",
    "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
    "onlineSupportSiteName": "Online Support Site Name value",
    "themeColor": {
      "@odata.type": "microsoft.graph.rgbColor",
      "r": 1,
      "g": 1,
      "b": 1
    },
    "showLogo": true,
    "lightBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "darkBackgroundLogo": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "showNameNextToLogo": true,
    "showDisplayNameNextToLogo": true
  }
}
```



