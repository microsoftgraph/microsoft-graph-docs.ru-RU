# <a name="update-reportroot"></a><span data-ttu-id="1f7d6-101">Обновление объекта reportRoot</span><span class="sxs-lookup"><span data-stu-id="1f7d6-101">Update reportRoot</span></span>

> <span data-ttu-id="1f7d6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f7d6-103">Обновление свойств объекта [reportRoot](../resources/intune_deviceconfig_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1f7d6-103">Update the properties of a [calendar](../resources/intune_deviceconfig_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f7d6-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1f7d6-104">Prerequisites</span></span>
<span data-ttu-id="1f7d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1f7d6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f7d6-107">Permission type</span></span>|<span data-ttu-id="1f7d6-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f7d6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f7d6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f7d6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1f7d6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f7d6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f7d6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f7d6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f7d6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-112">Not supported.</span></span>|
|<span data-ttu-id="1f7d6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f7d6-113">Application</span></span>|<span data-ttu-id="1f7d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f7d6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f7d6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="1f7d6-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f7d6-116">Request headers</span></span>
|<span data-ttu-id="1f7d6-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f7d6-117">Header</span></span>|<span data-ttu-id="1f7d6-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1f7d6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f7d6-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f7d6-119">Authorization</span></span>|<span data-ttu-id="1f7d6-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f7d6-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1f7d6-121">Accept</span></span>|<span data-ttu-id="1f7d6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1f7d6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f7d6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f7d6-123">Request body</span></span>
<span data-ttu-id="1f7d6-124">В тексте запроса добавьте представление объекта [reportRoot](../resources/intune_deviceconfig_reportroot.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_reportroot.md) object.</span></span>

<span data-ttu-id="1f7d6-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [reportRoot](../resources/intune_deviceconfig_reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1f7d6-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1f7d6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f7d6-126">Property</span></span>|<span data-ttu-id="1f7d6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1f7d6-127">Type</span></span>|<span data-ttu-id="1f7d6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7d6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f7d6-129">id</span><span class="sxs-lookup"><span data-stu-id="1f7d6-129">id</span></span>|<span data-ttu-id="1f7d6-130">String</span><span class="sxs-lookup"><span data-stu-id="1f7d6-130">String</span></span>|<span data-ttu-id="1f7d6-131">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-131">The unique identifier for this trace message.</span></span>|



## <a name="response"></a><span data-ttu-id="1f7d6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f7d6-132">Response</span></span>
<span data-ttu-id="1f7d6-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [reportRoot](../resources/intune_deviceconfig_reportroot.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f7d6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1f7d6-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f7d6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f7d6-135">Request</span></span>
<span data-ttu-id="1f7d6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="1f7d6-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f7d6-137">Response</span></span>
<span data-ttu-id="1f7d6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1f7d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



