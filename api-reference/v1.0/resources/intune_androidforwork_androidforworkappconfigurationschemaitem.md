# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="4ead5-101">Тип ресурса androidForWorkAppConfigurationSchemaItem</span><span class="sxs-lookup"><span data-stu-id="4ead5-101">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="4ead5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ead5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ead5-103">Один элемент конфигурации в схеме настраиваемой конфигурации Android for Work.</span><span class="sxs-lookup"><span data-stu-id="4ead5-103">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="4ead5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ead5-104">Properties</span></span>
|<span data-ttu-id="4ead5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ead5-105">Property</span></span>|<span data-ttu-id="4ead5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4ead5-106">Type</span></span>|<span data-ttu-id="4ead5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4ead5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ead5-108">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="4ead5-108">schemaItemKey</span></span>|<span data-ttu-id="4ead5-109">String</span><span class="sxs-lookup"><span data-stu-id="4ead5-109">String</span></span>|<span data-ttu-id="4ead5-110">Уникальный ключ, используемый приложением для определения элемента.</span><span class="sxs-lookup"><span data-stu-id="4ead5-110">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="4ead5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4ead5-111">displayName</span></span>|<span data-ttu-id="4ead5-112">String</span><span class="sxs-lookup"><span data-stu-id="4ead5-112">String</span></span>|<span data-ttu-id="4ead5-113">Понятное человеку имя.</span><span class="sxs-lookup"><span data-stu-id="4ead5-113">Human readable name</span></span>|
|<span data-ttu-id="4ead5-114">description</span><span class="sxs-lookup"><span data-stu-id="4ead5-114">description</span></span>|<span data-ttu-id="4ead5-115">String</span><span class="sxs-lookup"><span data-stu-id="4ead5-115">String</span></span>|<span data-ttu-id="4ead5-116">Описание компонентов приложения, которыми управляет элемент.</span><span class="sxs-lookup"><span data-stu-id="4ead5-116">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="4ead5-117">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="4ead5-117">defaultBoolValue</span></span>|<span data-ttu-id="4ead5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ead5-118">Boolean</span></span>|<span data-ttu-id="4ead5-119">Значение по умолчанию для элементов логического типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4ead5-119">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4ead5-120">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="4ead5-120">defaultIntValue</span></span>|<span data-ttu-id="4ead5-121">Int32</span><span class="sxs-lookup"><span data-stu-id="4ead5-121">Int32</span></span>|<span data-ttu-id="4ead5-122">Значение по умолчанию для элементов целочисленного типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4ead5-122">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4ead5-123">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="4ead5-123">defaultStringValue</span></span>|<span data-ttu-id="4ead5-124">String</span><span class="sxs-lookup"><span data-stu-id="4ead5-124">String</span></span>|<span data-ttu-id="4ead5-125">Значение по умолчанию для элементов строкового типа, если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4ead5-125">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4ead5-126">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="4ead5-126">defaultStringArrayValue</span></span>|<span data-ttu-id="4ead5-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4ead5-127">String collection</span></span>|<span data-ttu-id="4ead5-128">Значение по умолчанию для элементов типа "массив строк", если указано разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4ead5-128">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="4ead5-129">dataType</span><span class="sxs-lookup"><span data-stu-id="4ead5-129">dataType</span></span>|<span data-ttu-id="4ead5-130">String</span><span class="sxs-lookup"><span data-stu-id="4ead5-130">String</span></span>|<span data-ttu-id="4ead5-131">Тип значения, описываемый элементом. Возможные значения: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span><span class="sxs-lookup"><span data-stu-id="4ead5-131">The type of value this item describes Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="4ead5-132">selections</span><span class="sxs-lookup"><span data-stu-id="4ead5-132">selections</span></span>|<span data-ttu-id="4ead5-133">Коллекция объектов [keyValuePair](../resources/intune_androidforwork_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4ead5-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) collection</span></span>|<span data-ttu-id="4ead5-134">Список понятных человеку пар имя-значение для допустимых значений, которые можно задать для этого элемента (только для элементов одиночного и множественного выбора).</span><span class="sxs-lookup"><span data-stu-id="4ead5-134">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ead5-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4ead5-135">Relationships</span></span>
<span data-ttu-id="4ead5-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4ead5-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ead5-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ead5-137">JSON Representation</span></span>
<span data-ttu-id="4ead5-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ead5-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



