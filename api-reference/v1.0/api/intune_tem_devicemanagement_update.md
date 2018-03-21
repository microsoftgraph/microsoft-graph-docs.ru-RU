# <a name="update-devicemanagement"></a><span data-ttu-id="7bb75-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="7bb75-101">Update deviceManagement</span></span>

> <span data-ttu-id="7bb75-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7bb75-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bb75-103">Обновление свойств объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7bb75-103">Update the properties of a [calendar](../resources/intune_tem_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bb75-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7bb75-104">Prerequisites</span></span>
<span data-ttu-id="7bb75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7bb75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bb75-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bb75-107">Permission type</span></span>|<span data-ttu-id="7bb75-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bb75-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bb75-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bb75-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7bb75-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bb75-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7bb75-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bb75-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bb75-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bb75-112">Not supported.</span></span>|
|<span data-ttu-id="7bb75-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bb75-113">Application</span></span>|<span data-ttu-id="7bb75-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bb75-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bb75-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bb75-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="7bb75-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bb75-116">Request headers</span></span>
|<span data-ttu-id="7bb75-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bb75-117">Header</span></span>|<span data-ttu-id="7bb75-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7bb75-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bb75-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bb75-119">Authorization</span></span>|<span data-ttu-id="7bb75-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bb75-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7bb75-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7bb75-121">Accept</span></span>|<span data-ttu-id="7bb75-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7bb75-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bb75-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bb75-123">Request body</span></span>
<span data-ttu-id="7bb75-124">В тексте запроса добавьте представление объекта [deviceManagement](../resources/intune_tem_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bb75-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_tem_devicemanagement.md) object.</span></span>

<span data-ttu-id="7bb75-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceManagement](../resources/intune_tem_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="7bb75-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7bb75-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bb75-126">Property</span></span>|<span data-ttu-id="7bb75-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7bb75-127">Type</span></span>|<span data-ttu-id="7bb75-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7bb75-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb75-129">id</span><span class="sxs-lookup"><span data-stu-id="7bb75-129">id</span></span>|<span data-ttu-id="7bb75-130">String</span><span class="sxs-lookup"><span data-stu-id="7bb75-130">String</span></span>|<span data-ttu-id="7bb75-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7bb75-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7bb75-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bb75-132">Response</span></span>
<span data-ttu-id="7bb75-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_tem_devicemanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bb75-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_tem_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bb75-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7bb75-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bb75-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bb75-135">Request</span></span>
<span data-ttu-id="7bb75-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bb75-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="7bb75-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bb75-137">Response</span></span>
<span data-ttu-id="7bb75-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7bb75-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



