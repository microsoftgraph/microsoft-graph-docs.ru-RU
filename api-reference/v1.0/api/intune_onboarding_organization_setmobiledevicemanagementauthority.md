# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="ac651-101">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ac651-101">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="ac651-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac651-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac651-103">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="ac651-103">Set mobile device management authority</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac651-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac651-104">Prerequisites</span></span>
<span data-ttu-id="ac651-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac651-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="ac651-107">Permission type</span></span>|<span data-ttu-id="ac651-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac651-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac651-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac651-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac651-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac651-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac651-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac651-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac651-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac651-112">Not supported.</span></span>|
|<span data-ttu-id="ac651-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac651-113">Application</span></span>|<span data-ttu-id="ac651-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac651-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac651-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac651-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="ac651-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac651-116">Request headers</span></span>
|<span data-ttu-id="ac651-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac651-117">Header</span></span>|<span data-ttu-id="ac651-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ac651-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac651-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac651-119">Authorization</span></span>|<span data-ttu-id="ac651-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac651-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac651-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ac651-121">Accept</span></span>|<span data-ttu-id="ac651-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac651-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac651-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac651-123">Request body</span></span>
<span data-ttu-id="ac651-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac651-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac651-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac651-125">Response</span></span>
<span data-ttu-id="ac651-126">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac651-126">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac651-127">Пример</span><span class="sxs-lookup"><span data-stu-id="ac651-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac651-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac651-128">Request</span></span>
<span data-ttu-id="ac651-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac651-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="ac651-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac651-130">Response</span></span>
<span data-ttu-id="ac651-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ac651-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```



