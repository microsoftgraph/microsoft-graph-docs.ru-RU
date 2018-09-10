# <a name="targetapps-action"></a><span data-ttu-id="941d3-101">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="941d3-101">targetApps action</span></span>

> <span data-ttu-id="941d3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="941d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="941d3-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="941d3-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="941d3-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="941d3-104">Prerequisites</span></span>
<span data-ttu-id="941d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="941d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="941d3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941d3-107">Permission type</span></span>|<span data-ttu-id="941d3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="941d3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="941d3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941d3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="941d3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941d3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="941d3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941d3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="941d3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941d3-112">Not supported.</span></span>|
|<span data-ttu-id="941d3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941d3-113">Application</span></span>|<span data-ttu-id="941d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941d3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="941d3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941d3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="941d3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941d3-116">Request headers</span></span>
|<span data-ttu-id="941d3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="941d3-117">Header</span></span>|<span data-ttu-id="941d3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="941d3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="941d3-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941d3-119">Authorization</span></span>|<span data-ttu-id="941d3-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="941d3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="941d3-121">Принять</span><span class="sxs-lookup"><span data-stu-id="941d3-121">Accept</span></span>|<span data-ttu-id="941d3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="941d3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="941d3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="941d3-123">Request body</span></span>
<span data-ttu-id="941d3-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="941d3-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="941d3-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="941d3-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="941d3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="941d3-126">Property</span></span>|<span data-ttu-id="941d3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="941d3-127">Type</span></span>|<span data-ttu-id="941d3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="941d3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="941d3-129">apps</span><span class="sxs-lookup"><span data-stu-id="941d3-129">apps</span></span>|<span data-ttu-id="941d3-130">Коллекция [managedMobileApp](../resources/intune_mam_managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="941d3-130">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) collection</span></span>|<span data-ttu-id="941d3-131">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="941d3-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="941d3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="941d3-132">Response</span></span>
<span data-ttu-id="941d3-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="941d3-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="941d3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="941d3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="941d3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="941d3-135">Request</span></span>
<span data-ttu-id="941d3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="941d3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="941d3-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="941d3-137">Response</span></span>
<span data-ttu-id="941d3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="941d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








