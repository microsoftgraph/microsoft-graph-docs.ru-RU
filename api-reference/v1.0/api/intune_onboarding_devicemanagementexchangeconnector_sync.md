# <a name="sync-action"></a><span data-ttu-id="ebc7c-101">Действие sync</span><span class="sxs-lookup"><span data-stu-id="ebc7c-101">sync action</span></span>

> <span data-ttu-id="ebc7c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebc7c-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ebc7c-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebc7c-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc7c-104">Prerequisites</span></span>
<span data-ttu-id="ebc7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ebc7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebc7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc7c-107">Permission type</span></span>|<span data-ttu-id="ebc7c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebc7c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebc7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebc7c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ebc7c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebc7c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebc7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebc7c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebc7c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-112">Not supported.</span></span>|
|<span data-ttu-id="ebc7c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebc7c-113">Application</span></span>|<span data-ttu-id="ebc7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebc7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebc7c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="ebc7c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebc7c-116">Request headers</span></span>
|<span data-ttu-id="ebc7c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebc7c-117">Header</span></span>|<span data-ttu-id="ebc7c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ebc7c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebc7c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebc7c-119">Authorization</span></span>|<span data-ttu-id="ebc7c-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ebc7c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebc7c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ebc7c-121">Accept</span></span>|<span data-ttu-id="ebc7c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ebc7c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebc7c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebc7c-123">Request body</span></span>
<span data-ttu-id="ebc7c-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ebc7c-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ebc7c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebc7c-126">Property</span></span>|<span data-ttu-id="ebc7c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc7c-127">Type</span></span>|<span data-ttu-id="ebc7c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc7c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc7c-129">syncType</span><span class="sxs-lookup"><span data-stu-id="ebc7c-129">syncType</span></span>|[<span data-ttu-id="ebc7c-130">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="ebc7c-130">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="ebc7c-131">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="ebc7c-131">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="ebc7c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebc7c-132">Response</span></span>
<span data-ttu-id="ebc7c-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebc7c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ebc7c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="ebc7c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebc7c-135">Request</span></span>
<span data-ttu-id="ebc7c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="ebc7c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebc7c-137">Response</span></span>
<span data-ttu-id="ebc7c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebc7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



