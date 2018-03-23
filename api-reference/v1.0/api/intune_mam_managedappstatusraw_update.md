# <a name="update-managedappstatusraw"></a><span data-ttu-id="ed362-101">Обновление объекта managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="ed362-101">Update managedAppStatusRaw</span></span>

> <span data-ttu-id="ed362-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed362-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed362-103">Обновление свойств объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-103">Update the properties of a [calendar](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed362-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ed362-104">Prerequisites</span></span>
<span data-ttu-id="ed362-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ed362-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed362-107">Permission type</span></span>|<span data-ttu-id="ed362-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed362-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed362-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed362-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ed362-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed362-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed362-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed362-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed362-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed362-112">Not supported.</span></span>|
|<span data-ttu-id="ed362-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed362-113">Application</span></span>|<span data-ttu-id="ed362-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed362-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed362-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed362-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ed362-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed362-116">Request headers</span></span>
|<span data-ttu-id="ed362-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed362-117">Header</span></span>|<span data-ttu-id="ed362-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ed362-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed362-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed362-119">Authorization</span></span>|<span data-ttu-id="ed362-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed362-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ed362-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ed362-121">Accept</span></span>|<span data-ttu-id="ed362-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ed362-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed362-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed362-123">Request body</span></span>
<span data-ttu-id="ed362-124">В теле запроса добавьте представление объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed362-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedappstatusraw.md) object.</span></span>

<span data-ttu-id="ed362-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ed362-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed362-126">Property</span></span>|<span data-ttu-id="ed362-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ed362-127">Type</span></span>|<span data-ttu-id="ed362-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ed362-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed362-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ed362-129">displayName</span></span>|<span data-ttu-id="ed362-130">String</span><span class="sxs-lookup"><span data-stu-id="ed362-130">String</span></span>|<span data-ttu-id="ed362-131">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="ed362-131">Friendly name of the status report.</span></span> <span data-ttu-id="ed362-132">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="ed362-133">id</span><span class="sxs-lookup"><span data-stu-id="ed362-133">id</span></span>|<span data-ttu-id="ed362-134">String</span><span class="sxs-lookup"><span data-stu-id="ed362-134">String</span></span>|<span data-ttu-id="ed362-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed362-135">Key of the setting.</span></span> <span data-ttu-id="ed362-136">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="ed362-137">version</span><span class="sxs-lookup"><span data-stu-id="ed362-137">version</span></span>|<span data-ttu-id="ed362-138">String</span><span class="sxs-lookup"><span data-stu-id="ed362-138">String</span></span>|<span data-ttu-id="ed362-139">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ed362-139">Version of the entity.</span></span> <span data-ttu-id="ed362-140">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ed362-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="ed362-141">content</span><span class="sxs-lookup"><span data-stu-id="ed362-141">content</span></span>|[<span data-ttu-id="ed362-142">Json</span><span class="sxs-lookup"><span data-stu-id="ed362-142">JSON</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="ed362-143">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="ed362-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="ed362-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed362-144">Response</span></span>
<span data-ttu-id="ed362-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ed362-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed362-146">Пример</span><span class="sxs-lookup"><span data-stu-id="ed362-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed362-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed362-147">Request</span></span>
<span data-ttu-id="ed362-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed362-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
Content-type: application/json
Content-length: 139

{
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="ed362-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed362-149">Response</span></span>
<span data-ttu-id="ed362-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed362-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



