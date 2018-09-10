# <a name="delete-resourceoperation"></a><span data-ttu-id="336ad-101">Удаление resourceOperation</span><span class="sxs-lookup"><span data-stu-id="336ad-101">Delete resourceOperation</span></span>

> <span data-ttu-id="336ad-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="336ad-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="336ad-103">Удаление объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="336ad-103">Deletes a [resourceOperation](../resources/intune_rbac_resourceoperation.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="336ad-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="336ad-104">Prerequisites</span></span>
<span data-ttu-id="336ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="336ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="336ad-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="336ad-107">Permission type</span></span>|<span data-ttu-id="336ad-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="336ad-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="336ad-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="336ad-109">Delegated (work or school account)</span></span>|<span data-ttu-id="336ad-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="336ad-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="336ad-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="336ad-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="336ad-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="336ad-112">Not supported.</span></span>|
|<span data-ttu-id="336ad-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="336ad-113">Application</span></span>|<span data-ttu-id="336ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="336ad-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="336ad-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="336ad-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="336ad-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="336ad-116">Request headers</span></span>
|<span data-ttu-id="336ad-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="336ad-117">Header</span></span>|<span data-ttu-id="336ad-118">Значение</span><span class="sxs-lookup"><span data-stu-id="336ad-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="336ad-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="336ad-119">Authorization</span></span>|<span data-ttu-id="336ad-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="336ad-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="336ad-121">Принять</span><span class="sxs-lookup"><span data-stu-id="336ad-121">Accept</span></span>|<span data-ttu-id="336ad-122">application/json</span><span class="sxs-lookup"><span data-stu-id="336ad-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="336ad-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="336ad-123">Request body</span></span>
<span data-ttu-id="336ad-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="336ad-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="336ad-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="336ad-125">Response</span></span>
<span data-ttu-id="336ad-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="336ad-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="336ad-127">Пример</span><span class="sxs-lookup"><span data-stu-id="336ad-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="336ad-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="336ad-128">Request</span></span>
<span data-ttu-id="336ad-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="336ad-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="336ad-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="336ad-130">Response</span></span>
<span data-ttu-id="336ad-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="336ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








