# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="0b63f-101">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="0b63f-101">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="0b63f-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0b63f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b63f-103">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b63f-103">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b63f-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b63f-104">Prerequisites</span></span>
<span data-ttu-id="0b63f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b63f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b63f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b63f-107">Permission type</span></span>|<span data-ttu-id="0b63f-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b63f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b63f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b63f-109">Delegated (work or school account)</span></span>| <span data-ttu-id="0b63f-110">_Изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="0b63f-110">_varies by context_</span></span>|
| <span data-ttu-id="0b63f-111">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="0b63f-111">.mam</span></span> | <span data-ttu-id="0b63f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b63f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="0b63f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b63f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b63f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b63f-114">Not supported.</span></span>|
|<span data-ttu-id="0b63f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b63f-115">Application</span></span>|<span data-ttu-id="0b63f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b63f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b63f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b63f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0b63f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b63f-118">Request headers</span></span>
|<span data-ttu-id="0b63f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b63f-119">Header</span></span>|<span data-ttu-id="0b63f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0b63f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b63f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b63f-121">Authorization</span></span>|<span data-ttu-id="0b63f-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="0b63f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b63f-123">Принять</span><span class="sxs-lookup"><span data-stu-id="0b63f-123">Accept</span></span>|<span data-ttu-id="0b63f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b63f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b63f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b63f-125">Request body</span></span>
<span data-ttu-id="0b63f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b63f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b63f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b63f-127">Response</span></span>
<span data-ttu-id="0b63f-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b63f-128">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b63f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0b63f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b63f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b63f-130">Request</span></span>
<span data-ttu-id="0b63f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b63f-131">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="0b63f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b63f-132">Response</span></span>
<span data-ttu-id="0b63f-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b63f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



