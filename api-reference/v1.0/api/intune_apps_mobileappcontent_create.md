# <a name="create-mobileappcontent"></a><span data-ttu-id="3ecfa-101">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="3ecfa-101">Create mobileAppContent</span></span>

> <span data-ttu-id="3ecfa-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ecfa-103">Создание объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="3ecfa-103">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ecfa-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3ecfa-104">Prerequisites</span></span>
<span data-ttu-id="3ecfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ecfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3ecfa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ecfa-107">Permission type</span></span>|<span data-ttu-id="3ecfa-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ecfa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ecfa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ecfa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3ecfa-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ecfa-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ecfa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ecfa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ecfa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-112">Not supported.</span></span>|
|<span data-ttu-id="3ecfa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ecfa-113">Application</span></span>|<span data-ttu-id="3ecfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ecfa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ecfa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="3ecfa-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ecfa-116">Request headers</span></span>
|<span data-ttu-id="3ecfa-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ecfa-117">Header</span></span>|<span data-ttu-id="3ecfa-118">Значение</span><span class="sxs-lookup"><span data-stu-id="3ecfa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ecfa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ecfa-119">Authorization</span></span>|<span data-ttu-id="3ecfa-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ecfa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3ecfa-121">Accept</span></span>|<span data-ttu-id="3ecfa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3ecfa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ecfa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ecfa-123">Request body</span></span>
<span data-ttu-id="3ecfa-124">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-124">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="3ecfa-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-125">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="3ecfa-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ecfa-126">Property</span></span>|<span data-ttu-id="3ecfa-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3ecfa-127">Type</span></span>|<span data-ttu-id="3ecfa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3ecfa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ecfa-129">id</span><span class="sxs-lookup"><span data-stu-id="3ecfa-129">id</span></span>|<span data-ttu-id="3ecfa-130">String</span><span class="sxs-lookup"><span data-stu-id="3ecfa-130">String</span></span>|<span data-ttu-id="3ecfa-131">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="3ecfa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ecfa-132">Response</span></span>
<span data-ttu-id="3ecfa-133">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune_apps_mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-133">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ecfa-134">Пример</span><span class="sxs-lookup"><span data-stu-id="3ecfa-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ecfa-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ecfa-135">Request</span></span>
<span data-ttu-id="3ecfa-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="3ecfa-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ecfa-137">Response</span></span>
<span data-ttu-id="3ecfa-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3ecfa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



