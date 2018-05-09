# <a name="create-managedappstatusraw"></a><span data-ttu-id="f60c1-101">Создание объекта managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f60c1-101">Create managedAppStatusRaw</span></span>

> <span data-ttu-id="f60c1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f60c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f60c1-103">Создание объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="f60c1-103">Create a new [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f60c1-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f60c1-104">Prerequisites</span></span>
<span data-ttu-id="f60c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f60c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f60c1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f60c1-107">Permission type</span></span>|<span data-ttu-id="f60c1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f60c1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f60c1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f60c1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f60c1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f60c1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f60c1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f60c1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f60c1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f60c1-112">Not supported.</span></span>|
|<span data-ttu-id="f60c1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f60c1-113">Application</span></span>|<span data-ttu-id="f60c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f60c1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f60c1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f60c1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f60c1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f60c1-116">Request headers</span></span>
|<span data-ttu-id="f60c1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f60c1-117">Header</span></span>|<span data-ttu-id="f60c1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f60c1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f60c1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f60c1-119">Authorization</span></span>|<span data-ttu-id="f60c1-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f60c1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f60c1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f60c1-121">Accept</span></span>|<span data-ttu-id="f60c1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f60c1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f60c1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f60c1-123">Request body</span></span>
<span data-ttu-id="f60c1-124">В теле запроса добавьте представление объекта managedAppStatusRaw в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f60c1-124">In the request body, supply a JSON representation for the managedAppStatusRaw object.</span></span>

<span data-ttu-id="f60c1-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppStatusRaw.</span><span class="sxs-lookup"><span data-stu-id="f60c1-125">The following table shows the properties that are required when you create the managedAppStatusRaw.</span></span>

|<span data-ttu-id="f60c1-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f60c1-126">Property</span></span>|<span data-ttu-id="f60c1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f60c1-127">Type</span></span>|<span data-ttu-id="f60c1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f60c1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f60c1-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f60c1-129">displayName</span></span>|<span data-ttu-id="f60c1-130">String</span><span class="sxs-lookup"><span data-stu-id="f60c1-130">String</span></span>|<span data-ttu-id="f60c1-131">Понятное имя отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="f60c1-131">Friendly name of the status report.</span></span> <span data-ttu-id="f60c1-132">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f60c1-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="f60c1-133">id</span><span class="sxs-lookup"><span data-stu-id="f60c1-133">id</span></span>|<span data-ttu-id="f60c1-134">String</span><span class="sxs-lookup"><span data-stu-id="f60c1-134">String</span></span>|<span data-ttu-id="f60c1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f60c1-135">Key of the entity.</span></span> <span data-ttu-id="f60c1-136">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f60c1-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="f60c1-137">version</span><span class="sxs-lookup"><span data-stu-id="f60c1-137">version</span></span>|<span data-ttu-id="f60c1-138">String</span><span class="sxs-lookup"><span data-stu-id="f60c1-138">String</span></span>|<span data-ttu-id="f60c1-139">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="f60c1-139">Version of the entity.</span></span> <span data-ttu-id="f60c1-140">Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f60c1-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="f60c1-141">content</span><span class="sxs-lookup"><span data-stu-id="f60c1-141">content</span></span>|[<span data-ttu-id="f60c1-142">Json</span><span class="sxs-lookup"><span data-stu-id="f60c1-142">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="f60c1-143">Содержимое отчета о состоянии.</span><span class="sxs-lookup"><span data-stu-id="f60c1-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="f60c1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f60c1-144">Response</span></span>
<span data-ttu-id="f60c1-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f60c1-145">If successful, this method returns a `201 Created` response code and a [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f60c1-146">Пример</span><span class="sxs-lookup"><span data-stu-id="f60c1-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f60c1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f60c1-147">Request</span></span>
<span data-ttu-id="f60c1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f60c1-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="f60c1-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="f60c1-149">Response</span></span>
<span data-ttu-id="f60c1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f60c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



