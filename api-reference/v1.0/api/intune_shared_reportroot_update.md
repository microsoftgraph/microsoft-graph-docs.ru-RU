# <a name="update-reportroot"></a><span data-ttu-id="e3abe-101">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="e3abe-101">Update reportRoot</span></span>

> <span data-ttu-id="e3abe-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3abe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3abe-103">Обновление свойств объекта [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="e3abe-103">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3abe-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e3abe-104">Prerequisites</span></span>
<span data-ttu-id="e3abe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e3abe-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3abe-107">Permission type</span></span>|<span data-ttu-id="e3abe-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3abe-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3abe-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3abe-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3abe-110">&nbsp; &nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="e3abe-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="e3abe-111">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3abe-111">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="e3abe-112">&nbsp; &nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="e3abe-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="e3abe-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3abe-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3abe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3abe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3abe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3abe-115">Not supported.</span></span>|
|<span data-ttu-id="e3abe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3abe-116">Application</span></span>|<span data-ttu-id="e3abe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3abe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3abe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3abe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="e3abe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3abe-119">Request headers</span></span>
|<span data-ttu-id="e3abe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3abe-120">Header</span></span>|<span data-ttu-id="e3abe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e3abe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3abe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3abe-122">Authorization</span></span>|<span data-ttu-id="e3abe-123">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="e3abe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3abe-124">Принять</span><span class="sxs-lookup"><span data-stu-id="e3abe-124">Accept</span></span>|<span data-ttu-id="e3abe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3abe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3abe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3abe-126">Request body</span></span>
<span data-ttu-id="e3abe-127">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune_shared_reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3abe-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

<span data-ttu-id="e3abe-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune_shared_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="e3abe-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune_shared_reportroot.md).</span></span>

|<span data-ttu-id="e3abe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3abe-129">Property</span></span>|<span data-ttu-id="e3abe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e3abe-130">Type</span></span>|<span data-ttu-id="e3abe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e3abe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3abe-132">id</span><span class="sxs-lookup"><span data-stu-id="e3abe-132">id</span></span>|<span data-ttu-id="e3abe-133">String</span><span class="sxs-lookup"><span data-stu-id="e3abe-133">String</span></span>|<span data-ttu-id="e3abe-134">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="e3abe-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e3abe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3abe-135">Response</span></span>
<span data-ttu-id="e3abe-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune_shared_reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3abe-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3abe-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e3abe-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3abe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3abe-138">Request</span></span>
<span data-ttu-id="e3abe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3abe-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="e3abe-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3abe-140">Response</span></span>
<span data-ttu-id="e3abe-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3abe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








