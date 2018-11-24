# <a name="sync-action"></a><span data-ttu-id="c032a-101">Действие sync</span><span class="sxs-lookup"><span data-stu-id="c032a-101">sync action</span></span>

> <span data-ttu-id="c032a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c032a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c032a-103">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c032a-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c032a-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c032a-104">Prerequisites</span></span>
<span data-ttu-id="c032a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c032a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c032a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c032a-107">Permission type</span></span>|<span data-ttu-id="c032a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c032a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c032a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c032a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c032a-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c032a-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c032a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c032a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c032a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c032a-112">Not supported.</span></span>|
|<span data-ttu-id="c032a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c032a-113">Application</span></span>|<span data-ttu-id="c032a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c032a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c032a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c032a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync
```

## <a name="request-headers"></a><span data-ttu-id="c032a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c032a-116">Request headers</span></span>
|<span data-ttu-id="c032a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c032a-117">Header</span></span>|<span data-ttu-id="c032a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c032a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c032a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c032a-119">Authorization</span></span>|<span data-ttu-id="c032a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c032a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c032a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c032a-121">Accept</span></span>|<span data-ttu-id="c032a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c032a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c032a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c032a-123">Request body</span></span>
<span data-ttu-id="c032a-124">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c032a-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c032a-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c032a-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c032a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c032a-126">Property</span></span>|<span data-ttu-id="c032a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c032a-127">Type</span></span>|<span data-ttu-id="c032a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c032a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c032a-129">syncType</span><span class="sxs-lookup"><span data-stu-id="c032a-129">syncType</span></span>|[<span data-ttu-id="c032a-130">deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="c032a-130">deviceManagementExchangeConnectorSyncType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorsynctype.md)|<span data-ttu-id="c032a-131">Тип выполняемой синхронизации (синхронизируется все или только изменения).</span><span class="sxs-lookup"><span data-stu-id="c032a-131">The type of sync which will be executed, full sync or delta sync.</span></span>|



## <a name="response"></a><span data-ttu-id="c032a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c032a-132">Response</span></span>
<span data-ttu-id="c032a-133">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c032a-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c032a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c032a-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="c032a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c032a-135">Request</span></span>
<span data-ttu-id="c032a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c032a-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}/sync

Content-type: application/json
Content-length: 31

{
  "syncType": "deltaSync"
}
```

### <a name="response"></a><span data-ttu-id="c032a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c032a-137">Response</span></span>
<span data-ttu-id="c032a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c032a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



