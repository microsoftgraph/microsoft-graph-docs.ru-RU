---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c08967a538577ccbaac68ab3964dea61dc18ac79
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798163"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="d0986-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="d0986-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="d0986-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0986-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0986-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0986-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0986-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d0986-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="d0986-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0986-107">Properties</span></span>
|<span data-ttu-id="d0986-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0986-108">Property</span></span>|<span data-ttu-id="d0986-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0986-109">Type</span></span>|<span data-ttu-id="d0986-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0986-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0986-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="d0986-111">appConfigKey</span></span>|<span data-ttu-id="d0986-112">String</span><span class="sxs-lookup"><span data-stu-id="d0986-112">String</span></span>|<span data-ttu-id="d0986-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d0986-113">app configuration key.</span></span>|
|<span data-ttu-id="d0986-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="d0986-114">appConfigKeyType</span></span>|[<span data-ttu-id="d0986-115">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="d0986-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="d0986-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d0986-116">app configuration key type.</span></span> <span data-ttu-id="d0986-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="d0986-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="d0986-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="d0986-118">appConfigKeyValue</span></span>|<span data-ttu-id="d0986-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d0986-119">String</span></span>|<span data-ttu-id="d0986-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d0986-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0986-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d0986-121">Relationships</span></span>
<span data-ttu-id="d0986-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d0986-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0986-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0986-123">JSON Representation</span></span>
<span data-ttu-id="d0986-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0986-124">Here is a JSON representation of the resource.</span></span>
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



