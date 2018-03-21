# <a name="create-mobileappcontent"></a><span data-ttu-id="c8166-101">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="c8166-101">Create mobileAppContent</span></span>

> <span data-ttu-id="c8166-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8166-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8166-103">Создание объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="c8166-103">Create a new [plannerBucket](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8166-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8166-104">Prerequisites</span></span>
<span data-ttu-id="c8166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c8166-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8166-107">Permission type</span></span>|<span data-ttu-id="c8166-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8166-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8166-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8166-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c8166-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8166-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8166-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8166-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8166-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8166-112">Not supported.</span></span>|
|<span data-ttu-id="c8166-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8166-113">Application</span></span>|<span data-ttu-id="c8166-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8166-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8166-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8166-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="c8166-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8166-116">Request headers</span></span>
|<span data-ttu-id="c8166-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8166-117">Header</span></span>|<span data-ttu-id="c8166-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c8166-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8166-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8166-119">Authorization</span></span>|<span data-ttu-id="c8166-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8166-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c8166-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c8166-121">Accept</span></span>|<span data-ttu-id="c8166-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c8166-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8166-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8166-123">Request body</span></span>
<span data-ttu-id="c8166-124">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8166-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="c8166-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="c8166-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c8166-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8166-126">Property</span></span>|<span data-ttu-id="c8166-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c8166-127">Type</span></span>|<span data-ttu-id="c8166-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c8166-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8166-129">id</span><span class="sxs-lookup"><span data-stu-id="c8166-129">id</span></span>|<span data-ttu-id="c8166-130">String</span><span class="sxs-lookup"><span data-stu-id="c8166-130">String</span></span>|<span data-ttu-id="c8166-131">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="c8166-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="c8166-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8166-132">Response</span></span>
<span data-ttu-id="c8166-133">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune_apps_mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8166-133">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8166-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c8166-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8166-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8166-135">Request</span></span>
<span data-ttu-id="c8166-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8166-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="c8166-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8166-137">Response</span></span>
<span data-ttu-id="c8166-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8166-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



