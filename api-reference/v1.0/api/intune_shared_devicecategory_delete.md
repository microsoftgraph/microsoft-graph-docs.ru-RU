# <a name="delete-devicecategory"></a><span data-ttu-id="d86f0-101">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d86f0-101">Delete deviceCategory</span></span>

> <span data-ttu-id="d86f0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d86f0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d86f0-103">Удаление объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d86f0-103">Deletes a [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d86f0-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d86f0-104">Prerequisites</span></span>
<span data-ttu-id="d86f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d86f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d86f0-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d86f0-107">Permission type</span></span>|<span data-ttu-id="d86f0-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d86f0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d86f0-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d86f0-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d86f0-110">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="d86f0-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d86f0-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86f0-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d86f0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d86f0-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d86f0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86f0-113">Not supported.</span></span>|
|<span data-ttu-id="d86f0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d86f0-114">Application</span></span>|<span data-ttu-id="d86f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86f0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d86f0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d86f0-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="d86f0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d86f0-117">Request headers</span></span>
|<span data-ttu-id="d86f0-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d86f0-118">Header</span></span>|<span data-ttu-id="d86f0-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d86f0-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d86f0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d86f0-120">Authorization</span></span>|<span data-ttu-id="d86f0-121">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d86f0-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d86f0-122">Accept</span><span class="sxs-lookup"><span data-stu-id="d86f0-122">Accept</span></span>|<span data-ttu-id="d86f0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="d86f0-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d86f0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d86f0-124">Request body</span></span>
<span data-ttu-id="d86f0-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d86f0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d86f0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="d86f0-126">Response</span></span>
<span data-ttu-id="d86f0-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d86f0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d86f0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d86f0-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="d86f0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d86f0-129">Request</span></span>
<span data-ttu-id="d86f0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d86f0-130">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="d86f0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d86f0-131">Response</span></span>
<span data-ttu-id="d86f0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d86f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



