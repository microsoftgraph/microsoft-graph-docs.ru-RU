# <a name="update-mobileappcategory"></a><span data-ttu-id="e1e99-101">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="e1e99-101">Update mobileAppCategory</span></span>

> <span data-ttu-id="e1e99-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1e99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1e99-103">Обновление свойств объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e1e99-103">Update the properties of a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1e99-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1e99-104">Prerequisites</span></span>
<span data-ttu-id="e1e99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1e99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e1e99-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1e99-107">Permission type</span></span>|<span data-ttu-id="e1e99-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1e99-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1e99-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1e99-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e1e99-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e99-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1e99-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1e99-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1e99-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e99-112">Not supported.</span></span>|
|<span data-ttu-id="e1e99-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1e99-113">Application</span></span>|<span data-ttu-id="e1e99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e99-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1e99-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1e99-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="e1e99-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1e99-116">Request headers</span></span>
|<span data-ttu-id="e1e99-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1e99-117">Header</span></span>|<span data-ttu-id="e1e99-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e1e99-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1e99-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1e99-119">Authorization</span></span>|<span data-ttu-id="e1e99-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="e1e99-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1e99-121">Принять</span><span class="sxs-lookup"><span data-stu-id="e1e99-121">Accept</span></span>|<span data-ttu-id="e1e99-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1e99-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1e99-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1e99-123">Request body</span></span>
<span data-ttu-id="e1e99-124">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1e99-124">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>

<span data-ttu-id="e1e99-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="e1e99-125">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).</span></span>

|<span data-ttu-id="e1e99-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1e99-126">Property</span></span>|<span data-ttu-id="e1e99-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e99-127">Type</span></span>|<span data-ttu-id="e1e99-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e99-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1e99-129">id</span><span class="sxs-lookup"><span data-stu-id="e1e99-129">id</span></span>|<span data-ttu-id="e1e99-130">Строка</span><span class="sxs-lookup"><span data-stu-id="e1e99-130">String</span></span>|<span data-ttu-id="e1e99-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1e99-131">The key of the entity.</span></span>|
|<span data-ttu-id="e1e99-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e1e99-132">displayName</span></span>|<span data-ttu-id="e1e99-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e1e99-133">String</span></span>|<span data-ttu-id="e1e99-134">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="e1e99-134">The name of the app category.</span></span>|
|<span data-ttu-id="e1e99-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1e99-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e1e99-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1e99-136">DateTimeOffset</span></span>|<span data-ttu-id="e1e99-137">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="e1e99-137">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="e1e99-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1e99-138">Response</span></span>
<span data-ttu-id="e1e99-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1e99-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1e99-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e1e99-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1e99-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1e99-141">Request</span></span>
<span data-ttu-id="e1e99-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1e99-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e1e99-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1e99-143">Response</span></span>
<span data-ttu-id="e1e99-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1e99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```








