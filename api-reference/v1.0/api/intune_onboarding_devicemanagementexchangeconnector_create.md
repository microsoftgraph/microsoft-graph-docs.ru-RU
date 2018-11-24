# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="95b7c-101">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="95b7c-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="95b7c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="95b7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95b7c-103">Создание объекта [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="95b7c-103">Create a new [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95b7c-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95b7c-104">Prerequisites</span></span>
<span data-ttu-id="95b7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="95b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="95b7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95b7c-107">Permission type</span></span>|<span data-ttu-id="95b7c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95b7c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95b7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95b7c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="95b7c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95b7c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="95b7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95b7c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95b7c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b7c-112">Not supported.</span></span>|
|<span data-ttu-id="95b7c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95b7c-113">Application</span></span>|<span data-ttu-id="95b7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b7c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95b7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95b7c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="95b7c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95b7c-116">Request headers</span></span>
|<span data-ttu-id="95b7c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95b7c-117">Header</span></span>|<span data-ttu-id="95b7c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="95b7c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95b7c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95b7c-119">Authorization</span></span>|<span data-ttu-id="95b7c-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95b7c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95b7c-121">Принять</span><span class="sxs-lookup"><span data-stu-id="95b7c-121">Accept</span></span>|<span data-ttu-id="95b7c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="95b7c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95b7c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95b7c-123">Request body</span></span>
<span data-ttu-id="95b7c-124">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95b7c-124">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="95b7c-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="95b7c-125">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="95b7c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="95b7c-126">Property</span></span>|<span data-ttu-id="95b7c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="95b7c-127">Type</span></span>|<span data-ttu-id="95b7c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="95b7c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b7c-129">id</span><span class="sxs-lookup"><span data-stu-id="95b7c-129">id</span></span>|<span data-ttu-id="95b7c-130">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-130">String</span></span>|<span data-ttu-id="95b7c-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="95b7c-131">Not yet documented</span></span>|
|<span data-ttu-id="95b7c-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="95b7c-132">lastSyncDateTime</span></span>|<span data-ttu-id="95b7c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95b7c-133">DateTimeOffset</span></span>|<span data-ttu-id="95b7c-134">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="95b7c-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="95b7c-135">status</span><span class="sxs-lookup"><span data-stu-id="95b7c-135">status</span></span>|[<span data-ttu-id="95b7c-136">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="95b7c-136">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="95b7c-137">Состояние соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="95b7c-137">Exchange Connector Status.</span></span> <span data-ttu-id="95b7c-138">Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="95b7c-138">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="95b7c-139">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="95b7c-139">primarySmtpAddress</span></span>|<span data-ttu-id="95b7c-140">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-140">String</span></span>|<span data-ttu-id="95b7c-141">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="95b7c-141">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="95b7c-142">serverName</span><span class="sxs-lookup"><span data-stu-id="95b7c-142">serverName</span></span>|<span data-ttu-id="95b7c-143">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-143">String</span></span>|<span data-ttu-id="95b7c-144">Имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="95b7c-144">The name of the Exchange server.</span></span>|
|<span data-ttu-id="95b7c-145">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="95b7c-145">connectorServerName</span></span>|<span data-ttu-id="95b7c-146">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-146">String</span></span>|<span data-ttu-id="95b7c-147">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="95b7c-147">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="95b7c-148">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="95b7c-148">exchangeConnectorType</span></span>|[<span data-ttu-id="95b7c-149">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="95b7c-149">deviceManagementExchangeConnectorType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|<span data-ttu-id="95b7c-150">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="95b7c-150">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="95b7c-151">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="95b7c-151">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="95b7c-152">version</span><span class="sxs-lookup"><span data-stu-id="95b7c-152">version</span></span>|<span data-ttu-id="95b7c-153">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-153">String</span></span>|<span data-ttu-id="95b7c-154">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="95b7c-154">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="95b7c-155">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="95b7c-155">exchangeAlias</span></span>|<span data-ttu-id="95b7c-156">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-156">String</span></span>|<span data-ttu-id="95b7c-157">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="95b7c-157">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="95b7c-158">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="95b7c-158">exchangeOrganization</span></span>|<span data-ttu-id="95b7c-159">String</span><span class="sxs-lookup"><span data-stu-id="95b7c-159">String</span></span>|<span data-ttu-id="95b7c-160">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="95b7c-160">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="95b7c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="95b7c-161">Response</span></span>
<span data-ttu-id="95b7c-162">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95b7c-162">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95b7c-163">Пример</span><span class="sxs-lookup"><span data-stu-id="95b7c-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="95b7c-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="95b7c-164">Request</span></span>
<span data-ttu-id="95b7c-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95b7c-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="95b7c-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="95b7c-166">Response</span></span>
<span data-ttu-id="95b7c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="95b7c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



