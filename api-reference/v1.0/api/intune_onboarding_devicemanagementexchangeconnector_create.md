# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="039e9-101">Создание объекта deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="039e9-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="039e9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="039e9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="039e9-103">Создание объекта [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="039e9-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="039e9-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="039e9-104">Prerequisites</span></span>
<span data-ttu-id="039e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="039e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="039e9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="039e9-107">Permission type</span></span>|<span data-ttu-id="039e9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="039e9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="039e9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="039e9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="039e9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039e9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="039e9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="039e9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="039e9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039e9-112">Not supported.</span></span>|
|<span data-ttu-id="039e9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="039e9-113">Application</span></span>|<span data-ttu-id="039e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="039e9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="039e9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="039e9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="039e9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="039e9-116">Request headers</span></span>
|<span data-ttu-id="039e9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="039e9-117">Header</span></span>|<span data-ttu-id="039e9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="039e9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="039e9-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="039e9-119">Authorization</span></span>|<span data-ttu-id="039e9-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="039e9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="039e9-121">Принять</span><span class="sxs-lookup"><span data-stu-id="039e9-121">Accept</span></span>|<span data-ttu-id="039e9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="039e9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="039e9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="039e9-123">Request body</span></span>
<span data-ttu-id="039e9-124">В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="039e9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="039e9-125">Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.</span><span class="sxs-lookup"><span data-stu-id="039e9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="039e9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="039e9-126">Property</span></span>|<span data-ttu-id="039e9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="039e9-127">Type</span></span>|<span data-ttu-id="039e9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="039e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039e9-129">id</span><span class="sxs-lookup"><span data-stu-id="039e9-129">id</span></span>|<span data-ttu-id="039e9-130">String</span><span class="sxs-lookup"><span data-stu-id="039e9-130">String</span></span>|<span data-ttu-id="039e9-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="039e9-131">Not yet documented</span></span>|
|<span data-ttu-id="039e9-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="039e9-132">lastSyncDateTime</span></span>|<span data-ttu-id="039e9-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039e9-133">DateTimeOffset</span></span>|<span data-ttu-id="039e9-134">Время последней синхронизации соединителя Exchange</span><span class="sxs-lookup"><span data-stu-id="039e9-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="039e9-135">status</span><span class="sxs-lookup"><span data-stu-id="039e9-135">status</span></span>|<span data-ttu-id="039e9-136">String</span><span class="sxs-lookup"><span data-stu-id="039e9-136">String</span></span>|<span data-ttu-id="039e9-137">Состояние соединителя Exchange. Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.</span><span class="sxs-lookup"><span data-stu-id="039e9-137">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="039e9-138">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="039e9-138">primarySmtpAddress</span></span>|<span data-ttu-id="039e9-139">String</span><span class="sxs-lookup"><span data-stu-id="039e9-139">String</span></span>|<span data-ttu-id="039e9-140">Электронный адрес, используемый для настройки соединителя Exchange между службами.</span><span class="sxs-lookup"><span data-stu-id="039e9-140">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="039e9-141">serverName</span><span class="sxs-lookup"><span data-stu-id="039e9-141">ServerName</span></span>|<span data-ttu-id="039e9-142">String</span><span class="sxs-lookup"><span data-stu-id="039e9-142">String</span></span>|<span data-ttu-id="039e9-143">Имя сервера, на котором размещается соединитель Exchange.</span><span class="sxs-lookup"><span data-stu-id="039e9-143">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="039e9-144">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="039e9-144">exchangeConnectorType</span></span>|<span data-ttu-id="039e9-145">String</span><span class="sxs-lookup"><span data-stu-id="039e9-145">String</span></span>|<span data-ttu-id="039e9-146">Тип настраиваемого соединителя Exchange.</span><span class="sxs-lookup"><span data-stu-id="039e9-146">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="039e9-147">Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span><span class="sxs-lookup"><span data-stu-id="039e9-147">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="039e9-148">version</span><span class="sxs-lookup"><span data-stu-id="039e9-148">version</span></span>|<span data-ttu-id="039e9-149">String</span><span class="sxs-lookup"><span data-stu-id="039e9-149">String</span></span>|<span data-ttu-id="039e9-150">Версия объекта ExchangeConnectorAgent</span><span class="sxs-lookup"><span data-stu-id="039e9-150">The version of the message.</span></span>|
|<span data-ttu-id="039e9-151">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="039e9-151">exchangeAlias</span></span>|<span data-ttu-id="039e9-152">String</span><span class="sxs-lookup"><span data-stu-id="039e9-152">String</span></span>|<span data-ttu-id="039e9-153">Псевдоним, назначенный серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="039e9-153">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="039e9-154">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="039e9-154">exchangeOrganization</span></span>|<span data-ttu-id="039e9-155">String</span><span class="sxs-lookup"><span data-stu-id="039e9-155">String</span></span>|<span data-ttu-id="039e9-156">Организация Exchange, соответствующая серверу Exchange Server</span><span class="sxs-lookup"><span data-stu-id="039e9-156">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="039e9-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="039e9-157">Response</span></span>
<span data-ttu-id="039e9-158">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="039e9-158">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039e9-159">Пример</span><span class="sxs-lookup"><span data-stu-id="039e9-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="039e9-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="039e9-160">Request</span></span>
<span data-ttu-id="039e9-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="039e9-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 433

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="039e9-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="039e9-162">Response</span></span>
<span data-ttu-id="039e9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="039e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



