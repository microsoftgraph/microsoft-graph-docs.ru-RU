---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adfc465e607567c02f80b63760fa45e62466398b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950482"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a465b-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="a465b-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a465b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a465b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a465b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a465b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a465b-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a465b-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="a465b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a465b-107">Properties</span></span>
|<span data-ttu-id="a465b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a465b-108">Property</span></span>|<span data-ttu-id="a465b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a465b-109">Type</span></span>|<span data-ttu-id="a465b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a465b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a465b-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a465b-111">appConfigKey</span></span>|<span data-ttu-id="a465b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a465b-112">String</span></span>|<span data-ttu-id="a465b-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a465b-113">app configuration key.</span></span>|
|<span data-ttu-id="a465b-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a465b-114">appConfigKeyType</span></span>|[<span data-ttu-id="a465b-115">Мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="a465b-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="a465b-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a465b-116">app configuration key type.</span></span> <span data-ttu-id="a465b-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="a465b-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a465b-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a465b-118">appConfigKeyValue</span></span>|<span data-ttu-id="a465b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a465b-119">String</span></span>|<span data-ttu-id="a465b-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a465b-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a465b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a465b-121">Relationships</span></span>
<span data-ttu-id="a465b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a465b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a465b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a465b-123">JSON Representation</span></span>
<span data-ttu-id="a465b-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a465b-124">Here is a JSON representation of the resource.</span></span>
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




