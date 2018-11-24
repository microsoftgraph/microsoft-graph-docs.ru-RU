# <a name="assign-action"></a><span data-ttu-id="e6bd2-101">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e6bd2-101">assign action</span></span>

> <span data-ttu-id="e6bd2-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6bd2-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e6bd2-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6bd2-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6bd2-104">Prerequisites</span></span>
<span data-ttu-id="e6bd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6bd2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6bd2-107">Permission type</span></span>|<span data-ttu-id="e6bd2-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6bd2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6bd2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6bd2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e6bd2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6bd2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6bd2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6bd2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6bd2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-112">Not supported.</span></span>|
|<span data-ttu-id="e6bd2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6bd2-113">Application</span></span>|<span data-ttu-id="e6bd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6bd2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6bd2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="e6bd2-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e6bd2-116">Request headers</span></span>
|<span data-ttu-id="e6bd2-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6bd2-117">Header</span></span>|<span data-ttu-id="e6bd2-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e6bd2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6bd2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6bd2-119">Authorization</span></span>|<span data-ttu-id="e6bd2-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e6bd2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6bd2-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e6bd2-121">Accept</span></span>|<span data-ttu-id="e6bd2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e6bd2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6bd2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6bd2-123">Request body</span></span>
<span data-ttu-id="e6bd2-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e6bd2-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e6bd2-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6bd2-126">Property</span></span>|<span data-ttu-id="e6bd2-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e6bd2-127">Type</span></span>|<span data-ttu-id="e6bd2-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e6bd2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6bd2-129">assignments</span><span class="sxs-lookup"><span data-stu-id="e6bd2-129">assignments</span></span>|<span data-ttu-id="e6bd2-130">Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6bd2-130">[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="e6bd2-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e6bd2-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e6bd2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6bd2-132">Response</span></span>
<span data-ttu-id="e6bd2-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6bd2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e6bd2-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6bd2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6bd2-135">Request</span></span>
<span data-ttu-id="e6bd2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6bd2-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assign

Content-type: application/json
Content-length: 282

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e6bd2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6bd2-137">Response</span></span>
<span data-ttu-id="e6bd2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e6bd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



