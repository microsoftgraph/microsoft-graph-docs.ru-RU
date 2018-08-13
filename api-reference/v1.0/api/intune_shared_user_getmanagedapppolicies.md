# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="12a63-101">Функция getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="12a63-101">getManagedAppPolicies function</span></span>

> <span data-ttu-id="12a63-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12a63-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12a63-103">Получает ограничения для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="12a63-103">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12a63-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12a63-104">Prerequisites</span></span>
<span data-ttu-id="12a63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12a63-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a63-107">Permission type</span></span>|<span data-ttu-id="12a63-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a63-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a63-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a63-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12a63-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12a63-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12a63-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a63-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a63-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a63-112">Not supported.</span></span>|
|<span data-ttu-id="12a63-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a63-113">Application</span></span>|<span data-ttu-id="12a63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a63-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a63-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a63-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="12a63-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12a63-116">Request headers</span></span>
|<span data-ttu-id="12a63-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12a63-117">Header</span></span>|<span data-ttu-id="12a63-118">Значение</span><span class="sxs-lookup"><span data-stu-id="12a63-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a63-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="12a63-119">Authorization</span></span>|<span data-ttu-id="12a63-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12a63-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a63-121">Accept</span><span class="sxs-lookup"><span data-stu-id="12a63-121">Accept</span></span>|<span data-ttu-id="12a63-122">application/json</span><span class="sxs-lookup"><span data-stu-id="12a63-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a63-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12a63-123">Request body</span></span>
<span data-ttu-id="12a63-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12a63-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a63-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a63-125">Response</span></span>
<span data-ttu-id="12a63-126">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12a63-126">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a63-127">Пример</span><span class="sxs-lookup"><span data-stu-id="12a63-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a63-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a63-128">Request</span></span>
<span data-ttu-id="12a63-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a63-129">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="12a63-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a63-130">Response</span></span>
<span data-ttu-id="12a63-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="12a63-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```



