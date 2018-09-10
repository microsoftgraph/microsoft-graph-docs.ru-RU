# <a name="assign-action"></a><span data-ttu-id="54df3-101">Действие assign</span><span class="sxs-lookup"><span data-stu-id="54df3-101">assign action</span></span>

> <span data-ttu-id="54df3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54df3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54df3-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="54df3-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54df3-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="54df3-104">Prerequisites</span></span>
<span data-ttu-id="54df3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="54df3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="54df3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54df3-107">Permission type</span></span>|<span data-ttu-id="54df3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54df3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54df3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54df3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="54df3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54df3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54df3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54df3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54df3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54df3-112">Not supported.</span></span>|
|<span data-ttu-id="54df3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54df3-113">Application</span></span>|<span data-ttu-id="54df3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54df3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54df3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54df3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="54df3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54df3-116">Request headers</span></span>
|<span data-ttu-id="54df3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54df3-117">Header</span></span>|<span data-ttu-id="54df3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="54df3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54df3-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54df3-119">Authorization</span></span>|<span data-ttu-id="54df3-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="54df3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54df3-121">Принять</span><span class="sxs-lookup"><span data-stu-id="54df3-121">Accept</span></span>|<span data-ttu-id="54df3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="54df3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54df3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54df3-123">Request body</span></span>
<span data-ttu-id="54df3-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54df3-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="54df3-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="54df3-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="54df3-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="54df3-126">Property</span></span>|<span data-ttu-id="54df3-127">Тип</span><span class="sxs-lookup"><span data-stu-id="54df3-127">Type</span></span>|<span data-ttu-id="54df3-128">Описание</span><span class="sxs-lookup"><span data-stu-id="54df3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54df3-129">assignments</span><span class="sxs-lookup"><span data-stu-id="54df3-129">assignments</span></span>|<span data-ttu-id="54df3-130">Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="54df3-130">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="54df3-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="54df3-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="54df3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="54df3-132">Response</span></span>
<span data-ttu-id="54df3-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54df3-133">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54df3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="54df3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="54df3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="54df3-135">Request</span></span>
<span data-ttu-id="54df3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54df3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 277

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="54df3-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="54df3-137">Response</span></span>
<span data-ttu-id="54df3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54df3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```








