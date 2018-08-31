# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="92700-101">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="92700-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="92700-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92700-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92700-103">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="92700-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="92700-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="92700-104">Properties</span></span>
|<span data-ttu-id="92700-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="92700-105">Property</span></span>|<span data-ttu-id="92700-106">Тип</span><span class="sxs-lookup"><span data-stu-id="92700-106">Type</span></span>|<span data-ttu-id="92700-107">Описание</span><span class="sxs-lookup"><span data-stu-id="92700-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92700-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="92700-108">appConfigKey</span></span>|<span data-ttu-id="92700-109">Строка</span><span class="sxs-lookup"><span data-stu-id="92700-109">String</span></span>|<span data-ttu-id="92700-110">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="92700-110">app configuration key.</span></span>|
|<span data-ttu-id="92700-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="92700-111">appConfigKeyType</span></span>|<span data-ttu-id="92700-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="92700-112">mdmAppConfigKeyType</span></span>|<span data-ttu-id="92700-113">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="92700-113">app configuration key type.</span></span> <span data-ttu-id="92700-114">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="92700-114">The possible values are `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`, , , , , , , or .</span></span>|
|<span data-ttu-id="92700-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="92700-115">appConfigKeyValue</span></span>|<span data-ttu-id="92700-116">Строка</span><span class="sxs-lookup"><span data-stu-id="92700-116">String</span></span>|<span data-ttu-id="92700-117">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="92700-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92700-118">Связи</span><span class="sxs-lookup"><span data-stu-id="92700-118">Relationships</span></span>
<span data-ttu-id="92700-119">Нет</span><span class="sxs-lookup"><span data-stu-id="92700-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92700-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92700-120">JSON Representation</span></span>
<span data-ttu-id="92700-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92700-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



