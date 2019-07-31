---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c001e19758865e957cb3d72f3d49acf3387281a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006054"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="fc919-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="fc919-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="fc919-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc919-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc919-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc919-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fc919-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="fc919-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc919-107">Properties</span></span>
|<span data-ttu-id="fc919-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc919-108">Property</span></span>|<span data-ttu-id="fc919-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc919-109">Type</span></span>|<span data-ttu-id="fc919-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc919-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc919-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="fc919-111">appConfigKey</span></span>|<span data-ttu-id="fc919-112">String</span><span class="sxs-lookup"><span data-stu-id="fc919-112">String</span></span>|<span data-ttu-id="fc919-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fc919-113">app configuration key.</span></span>|
|<span data-ttu-id="fc919-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="fc919-114">appConfigKeyType</span></span>|[<span data-ttu-id="fc919-115">Мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="fc919-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="fc919-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fc919-116">app configuration key type.</span></span> <span data-ttu-id="fc919-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="fc919-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="fc919-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="fc919-118">appConfigKeyValue</span></span>|<span data-ttu-id="fc919-119">Строка</span><span class="sxs-lookup"><span data-stu-id="fc919-119">String</span></span>|<span data-ttu-id="fc919-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fc919-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc919-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc919-121">Relationships</span></span>
<span data-ttu-id="fc919-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fc919-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc919-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc919-123">JSON Representation</span></span>
<span data-ttu-id="fc919-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc919-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```





