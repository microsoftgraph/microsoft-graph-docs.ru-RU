# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="88b13-101">Обновление объекта androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="88b13-101">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="88b13-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="88b13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88b13-103">Обновление свойств объекта [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="88b13-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="88b13-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="88b13-104">Prerequisites</span></span>
<span data-ttu-id="88b13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="88b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="88b13-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88b13-107">Permission type</span></span>|<span data-ttu-id="88b13-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88b13-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88b13-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88b13-109">Delegated (work or school account)</span></span>|<span data-ttu-id="88b13-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88b13-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88b13-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88b13-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88b13-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88b13-112">Not supported.</span></span>|
|<span data-ttu-id="88b13-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88b13-113">Application</span></span>|<span data-ttu-id="88b13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88b13-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88b13-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88b13-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="88b13-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88b13-116">Request headers</span></span>
|<span data-ttu-id="88b13-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88b13-117">Header</span></span>|<span data-ttu-id="88b13-118">Значение</span><span class="sxs-lookup"><span data-stu-id="88b13-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88b13-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="88b13-119">Authorization</span></span>|<span data-ttu-id="88b13-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88b13-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88b13-121">Accept</span><span class="sxs-lookup"><span data-stu-id="88b13-121">Accept</span></span>|<span data-ttu-id="88b13-122">application/json</span><span class="sxs-lookup"><span data-stu-id="88b13-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88b13-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88b13-123">Request body</span></span>
<span data-ttu-id="88b13-124">В тексте запроса добавьте представление объекта [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88b13-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="88b13-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="88b13-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="88b13-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="88b13-126">Property</span></span>|<span data-ttu-id="88b13-127">Тип</span><span class="sxs-lookup"><span data-stu-id="88b13-127">Type</span></span>|<span data-ttu-id="88b13-128">Описание</span><span class="sxs-lookup"><span data-stu-id="88b13-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88b13-129">id</span><span class="sxs-lookup"><span data-stu-id="88b13-129">id</span></span>|<span data-ttu-id="88b13-130">String</span><span class="sxs-lookup"><span data-stu-id="88b13-130">String</span></span>|<span data-ttu-id="88b13-131">Ключ объекта, которому соответствует имя пакета Android для схемы приложений.</span><span class="sxs-lookup"><span data-stu-id="88b13-131">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="88b13-132">exampleJson</span><span class="sxs-lookup"><span data-stu-id="88b13-132">exampleJson</span></span>|<span data-ttu-id="88b13-133">Binary</span><span class="sxs-lookup"><span data-stu-id="88b13-133">Binary</span></span>|<span data-ttu-id="88b13-134">Массив байтов в кодировке UTF8, содержащий образец соответствующей схеме строки JSON, который иллюстрирует настройку приложения.</span><span class="sxs-lookup"><span data-stu-id="88b13-134">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="88b13-135">schemaItems</span><span class="sxs-lookup"><span data-stu-id="88b13-135">schemaItems</span></span>|<span data-ttu-id="88b13-136">Коллекция [androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md)</span><span class="sxs-lookup"><span data-stu-id="88b13-136">[androidForWorkAppConfigurationSchemaItem](../resources/intune_androidforwork_androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="88b13-137">Коллекция элементов, каждый из которых представляет именованный параметр конфигурации в схеме.</span><span class="sxs-lookup"><span data-stu-id="88b13-137">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="88b13-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="88b13-138">Response</span></span>
<span data-ttu-id="88b13-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkAppConfigurationSchema](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88b13-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88b13-140">Пример</span><span class="sxs-lookup"><span data-stu-id="88b13-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="88b13-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="88b13-141">Request</span></span>
<span data-ttu-id="88b13-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88b13-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 720

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="88b13-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="88b13-143">Response</span></span>
<span data-ttu-id="88b13-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="88b13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```



