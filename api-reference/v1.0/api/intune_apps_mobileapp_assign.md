# <a name="assign-action"></a><span data-ttu-id="70aed-101">Действие assign</span><span class="sxs-lookup"><span data-stu-id="70aed-101">assign action</span></span>

> <span data-ttu-id="70aed-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="70aed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70aed-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="70aed-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70aed-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="70aed-104">Prerequisites</span></span>
<span data-ttu-id="70aed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="70aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="70aed-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70aed-107">Permission type</span></span>|<span data-ttu-id="70aed-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70aed-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70aed-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70aed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="70aed-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70aed-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70aed-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70aed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70aed-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70aed-112">Not supported.</span></span>|
|<span data-ttu-id="70aed-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70aed-113">Application</span></span>|<span data-ttu-id="70aed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70aed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70aed-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70aed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="70aed-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="70aed-116">Request headers</span></span>
|<span data-ttu-id="70aed-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70aed-117">Header</span></span>|<span data-ttu-id="70aed-118">Значение</span><span class="sxs-lookup"><span data-stu-id="70aed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70aed-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="70aed-119">Authorization</span></span>|<span data-ttu-id="70aed-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70aed-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70aed-121">Accept</span><span class="sxs-lookup"><span data-stu-id="70aed-121">Accept</span></span>|<span data-ttu-id="70aed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="70aed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70aed-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70aed-123">Request body</span></span>
<span data-ttu-id="70aed-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70aed-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="70aed-125">В следующей таблице показаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="70aed-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="70aed-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="70aed-126">Property</span></span>|<span data-ttu-id="70aed-127">Тип</span><span class="sxs-lookup"><span data-stu-id="70aed-127">Type</span></span>|<span data-ttu-id="70aed-128">Описание</span><span class="sxs-lookup"><span data-stu-id="70aed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70aed-129">mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="70aed-129">mobileAppAssignments</span></span>|<span data-ttu-id="70aed-130">Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="70aed-130">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="70aed-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="70aed-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="70aed-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="70aed-132">Response</span></span>
<span data-ttu-id="70aed-133">В случае успешного выполнения этот метод возвращает код ответа `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="70aed-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70aed-134">Пример</span><span class="sxs-lookup"><span data-stu-id="70aed-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="70aed-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="70aed-135">Request</span></span>
<span data-ttu-id="70aed-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70aed-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assign

Content-type: application/json
Content-length: 406

{
  "mobileAppAssignments": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="70aed-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="70aed-137">Response</span></span>
<span data-ttu-id="70aed-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="70aed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



