---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b7145b7adf9aed622af8ebb3a6a55c6456d7e8a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356305"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="43e3b-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="43e3b-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="43e3b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43e3b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43e3b-105">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="43e3b-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="43e3b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="43e3b-106">Properties</span></span>
|<span data-ttu-id="43e3b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="43e3b-107">Property</span></span>|<span data-ttu-id="43e3b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="43e3b-108">Type</span></span>|<span data-ttu-id="43e3b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="43e3b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e3b-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="43e3b-110">appConfigKey</span></span>|<span data-ttu-id="43e3b-111">String</span><span class="sxs-lookup"><span data-stu-id="43e3b-111">String</span></span>|<span data-ttu-id="43e3b-112">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="43e3b-112">app configuration key.</span></span>|
|<span data-ttu-id="43e3b-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="43e3b-113">appConfigKeyType</span></span>|[<span data-ttu-id="43e3b-114">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="43e3b-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="43e3b-115">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="43e3b-115">app configuration key type.</span></span> <span data-ttu-id="43e3b-116">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="43e3b-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="43e3b-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="43e3b-117">appConfigKeyValue</span></span>|<span data-ttu-id="43e3b-118">Строка</span><span class="sxs-lookup"><span data-stu-id="43e3b-118">String</span></span>|<span data-ttu-id="43e3b-119">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="43e3b-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43e3b-120">Связи</span><span class="sxs-lookup"><span data-stu-id="43e3b-120">Relationships</span></span>
<span data-ttu-id="43e3b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="43e3b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43e3b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43e3b-122">JSON Representation</span></span>
<span data-ttu-id="43e3b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43e3b-123">Here is a JSON representation of the resource.</span></span>
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




