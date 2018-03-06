# <a name="delete-windows10mobilecompliancepolicy"></a><span data-ttu-id="fb0ee-101">Удаление объекта windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fb0ee-101">Delete windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="fb0ee-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb0ee-103">Удаляет экземпляр [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fb0ee-103">Deletes a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb0ee-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb0ee-104">Prerequisites</span></span>
<span data-ttu-id="fb0ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb0ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb0ee-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb0ee-107">Permission type</span></span>|<span data-ttu-id="fb0ee-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb0ee-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb0ee-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb0ee-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fb0ee-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb0ee-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb0ee-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb0ee-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb0ee-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-112">Not supported.</span></span>|
|<span data-ttu-id="fb0ee-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb0ee-113">Application</span></span>|<span data-ttu-id="fb0ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb0ee-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb0ee-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fb0ee-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb0ee-116">Request headers</span></span>
|<span data-ttu-id="fb0ee-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb0ee-117">Header</span></span>|<span data-ttu-id="fb0ee-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fb0ee-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb0ee-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb0ee-119">Authorization</span></span>|<span data-ttu-id="fb0ee-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fb0ee-121">Принять</span><span class="sxs-lookup"><span data-stu-id="fb0ee-121">Accept</span></span>|<span data-ttu-id="fb0ee-122">application/json</span><span class="sxs-lookup"><span data-stu-id="fb0ee-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb0ee-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb0ee-123">Request body</span></span>
<span data-ttu-id="fb0ee-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb0ee-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb0ee-125">Response</span></span>
<span data-ttu-id="fb0ee-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb0ee-127">Пример</span><span class="sxs-lookup"><span data-stu-id="fb0ee-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb0ee-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb0ee-128">Request</span></span>
<span data-ttu-id="fb0ee-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="fb0ee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb0ee-130">Response</span></span>
<span data-ttu-id="fb0ee-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb0ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



