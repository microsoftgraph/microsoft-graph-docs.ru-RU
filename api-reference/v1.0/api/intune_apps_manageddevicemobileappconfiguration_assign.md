# <a name="assign-action"></a><span data-ttu-id="0d81e-101">Действие assign</span><span class="sxs-lookup"><span data-stu-id="0d81e-101">assign action</span></span>

> <span data-ttu-id="0d81e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0d81e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d81e-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0d81e-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d81e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0d81e-104">Prerequisites</span></span>
<span data-ttu-id="0d81e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0d81e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0d81e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d81e-107">Permission type</span></span>|<span data-ttu-id="0d81e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d81e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d81e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d81e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0d81e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d81e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d81e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d81e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d81e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d81e-112">Not supported.</span></span>|
|<span data-ttu-id="0d81e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d81e-113">Application</span></span>|<span data-ttu-id="0d81e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d81e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d81e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d81e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="0d81e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d81e-116">Request headers</span></span>
|<span data-ttu-id="0d81e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d81e-117">Header</span></span>|<span data-ttu-id="0d81e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="0d81e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d81e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d81e-119">Authorization</span></span>|<span data-ttu-id="0d81e-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0d81e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d81e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0d81e-121">Accept</span></span>|<span data-ttu-id="0d81e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0d81e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d81e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d81e-123">Request body</span></span>
<span data-ttu-id="0d81e-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d81e-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0d81e-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0d81e-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0d81e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d81e-126">Property</span></span>|<span data-ttu-id="0d81e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0d81e-127">Type</span></span>|<span data-ttu-id="0d81e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0d81e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d81e-129">assignments</span><span class="sxs-lookup"><span data-stu-id="0d81e-129">assignments</span></span>|<span data-ttu-id="0d81e-130">Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0d81e-130">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0d81e-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0d81e-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0d81e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d81e-132">Response</span></span>
<span data-ttu-id="0d81e-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d81e-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d81e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0d81e-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d81e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d81e-135">Request</span></span>
<span data-ttu-id="0d81e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d81e-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0d81e-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d81e-137">Response</span></span>
<span data-ttu-id="0d81e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0d81e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



