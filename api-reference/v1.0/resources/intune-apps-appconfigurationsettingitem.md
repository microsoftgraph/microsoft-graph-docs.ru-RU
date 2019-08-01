---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91ccefc06ba6a635b9b18e07465ea0332c48f022
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030179"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="e45f0-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="e45f0-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="e45f0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e45f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e45f0-105">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e45f0-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="e45f0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e45f0-106">Properties</span></span>
|<span data-ttu-id="e45f0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e45f0-107">Property</span></span>|<span data-ttu-id="e45f0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e45f0-108">Type</span></span>|<span data-ttu-id="e45f0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e45f0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45f0-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="e45f0-110">appConfigKey</span></span>|<span data-ttu-id="e45f0-111">String</span><span class="sxs-lookup"><span data-stu-id="e45f0-111">String</span></span>|<span data-ttu-id="e45f0-112">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e45f0-112">app configuration key.</span></span>|
|<span data-ttu-id="e45f0-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e45f0-113">appConfigKeyType</span></span>|[<span data-ttu-id="e45f0-114">Мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="e45f0-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="e45f0-115">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e45f0-115">app configuration key type.</span></span> <span data-ttu-id="e45f0-116">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="e45f0-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="e45f0-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="e45f0-117">appConfigKeyValue</span></span>|<span data-ttu-id="e45f0-118">Строка</span><span class="sxs-lookup"><span data-stu-id="e45f0-118">String</span></span>|<span data-ttu-id="e45f0-119">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e45f0-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45f0-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="e45f0-120">Relationships</span></span>
<span data-ttu-id="e45f0-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e45f0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e45f0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e45f0-122">JSON Representation</span></span>
<span data-ttu-id="e45f0-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e45f0-123">Here is a JSON representation of the resource.</span></span>
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



