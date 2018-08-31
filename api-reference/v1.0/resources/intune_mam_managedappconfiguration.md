# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="bc203-101">Тип ресурса managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc203-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="bc203-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc203-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc203-103">Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация</span><span class="sxs-lookup"><span data-stu-id="bc203-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="bc203-104">Наследуется от [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc203-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bc203-105">Методы</span><span class="sxs-lookup"><span data-stu-id="bc203-105">Methods</span></span>
|<span data-ttu-id="bc203-106">Метод</span><span class="sxs-lookup"><span data-stu-id="bc203-106">Method</span></span>|<span data-ttu-id="bc203-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc203-107">Return Type</span></span>|<span data-ttu-id="bc203-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bc203-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc203-109">Список managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="bc203-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="bc203-110">Коллекция [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc203-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="bc203-111">Список свойств и связей объектов [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bc203-112">Получение объекта managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc203-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="bc203-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc203-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="bc203-114">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc203-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc203-115">Properties</span></span>
|<span data-ttu-id="bc203-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc203-116">Property</span></span>|<span data-ttu-id="bc203-117">Тип</span><span class="sxs-lookup"><span data-stu-id="bc203-117">Type</span></span>|<span data-ttu-id="bc203-118">Описание</span><span class="sxs-lookup"><span data-stu-id="bc203-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc203-119">displayName</span><span class="sxs-lookup"><span data-stu-id="bc203-119">displayName</span></span>|<span data-ttu-id="bc203-120">String</span><span class="sxs-lookup"><span data-stu-id="bc203-120">String</span></span>|<span data-ttu-id="bc203-121">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bc203-121">Policy display name.</span></span> <span data-ttu-id="bc203-122">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-123">description</span><span class="sxs-lookup"><span data-stu-id="bc203-123">description</span></span>|<span data-ttu-id="bc203-124">String</span><span class="sxs-lookup"><span data-stu-id="bc203-124">String</span></span>|<span data-ttu-id="bc203-125">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bc203-125">The policy's description.</span></span> <span data-ttu-id="bc203-126">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc203-127">createdDateTime</span></span>|<span data-ttu-id="bc203-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc203-128">DateTimeOffset</span></span>|<span data-ttu-id="bc203-129">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bc203-129">The date and time the policy was created.</span></span> <span data-ttu-id="bc203-130">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc203-131">lastModifiedDateTime</span></span>|<span data-ttu-id="bc203-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc203-132">DateTimeOffset</span></span>|<span data-ttu-id="bc203-133">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bc203-133">Last time the policy was modified.</span></span> <span data-ttu-id="bc203-134">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-135">id</span><span class="sxs-lookup"><span data-stu-id="bc203-135">id</span></span>|<span data-ttu-id="bc203-136">Строка</span><span class="sxs-lookup"><span data-stu-id="bc203-136">String</span></span>|<span data-ttu-id="bc203-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc203-137">Key of the entity.</span></span> <span data-ttu-id="bc203-138">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-139">version</span><span class="sxs-lookup"><span data-stu-id="bc203-139">version</span></span>|<span data-ttu-id="bc203-140">String</span><span class="sxs-lookup"><span data-stu-id="bc203-140">String</span></span>|<span data-ttu-id="bc203-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bc203-141">Version of the entity.</span></span> <span data-ttu-id="bc203-142">Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bc203-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="bc203-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="bc203-143">customSettings</span></span>|<span data-ttu-id="bc203-144">Коллекция [keyValuePair](../resources/intune_mam_keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bc203-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="bc203-145">Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой</span><span class="sxs-lookup"><span data-stu-id="bc203-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc203-146">Связи</span><span class="sxs-lookup"><span data-stu-id="bc203-146">Relationships</span></span>
<span data-ttu-id="bc203-147">Нет</span><span class="sxs-lookup"><span data-stu-id="bc203-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc203-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc203-148">JSON Representation</span></span>
<span data-ttu-id="bc203-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc203-149">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



