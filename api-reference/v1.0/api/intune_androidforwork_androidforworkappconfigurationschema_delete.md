# <a name="delete-androidforworkappconfigurationschema"></a><span data-ttu-id="8464b-101">Удаление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="8464b-101">Delete androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="8464b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8464b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8464b-103">Удаляет объект [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="8464b-103">Deletes a [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8464b-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8464b-104">Prerequisites</span></span>
<span data-ttu-id="8464b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8464b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8464b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8464b-107">Permission type</span></span>|<span data-ttu-id="8464b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8464b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8464b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8464b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8464b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8464b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8464b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8464b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8464b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8464b-112">Not supported.</span></span>|
|<span data-ttu-id="8464b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8464b-113">Application</span></span>|<span data-ttu-id="8464b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8464b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8464b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8464b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="8464b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8464b-116">Request headers</span></span>
|<span data-ttu-id="8464b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8464b-117">Header</span></span>|<span data-ttu-id="8464b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8464b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8464b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8464b-119">Authorization</span></span>|<span data-ttu-id="8464b-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8464b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8464b-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8464b-121">Accept</span></span>|<span data-ttu-id="8464b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8464b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8464b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8464b-123">Request body</span></span>
<span data-ttu-id="8464b-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8464b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8464b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8464b-125">Response</span></span>
<span data-ttu-id="8464b-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8464b-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8464b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8464b-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8464b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8464b-128">Request</span></span>
<span data-ttu-id="8464b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8464b-129">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="8464b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8464b-130">Response</span></span>
<span data-ttu-id="8464b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8464b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



