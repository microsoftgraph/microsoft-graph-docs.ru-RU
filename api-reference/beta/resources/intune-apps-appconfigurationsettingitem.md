---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f001a02a1e4e3ef2a15fe5e606687896775a6d26
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991263"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="03099-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="03099-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="03099-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03099-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03099-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03099-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="03099-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="03099-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="03099-107">Properties</span></span>
|<span data-ttu-id="03099-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="03099-108">Property</span></span>|<span data-ttu-id="03099-109">Тип</span><span class="sxs-lookup"><span data-stu-id="03099-109">Type</span></span>|<span data-ttu-id="03099-110">Описание</span><span class="sxs-lookup"><span data-stu-id="03099-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03099-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="03099-111">appConfigKey</span></span>|<span data-ttu-id="03099-112">String</span><span class="sxs-lookup"><span data-stu-id="03099-112">String</span></span>|<span data-ttu-id="03099-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="03099-113">app configuration key.</span></span>|
|<span data-ttu-id="03099-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="03099-114">appConfigKeyType</span></span>|[<span data-ttu-id="03099-115">Мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="03099-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="03099-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="03099-116">app configuration key type.</span></span> <span data-ttu-id="03099-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="03099-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="03099-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="03099-118">appConfigKeyValue</span></span>|<span data-ttu-id="03099-119">Строка</span><span class="sxs-lookup"><span data-stu-id="03099-119">String</span></span>|<span data-ttu-id="03099-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="03099-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03099-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="03099-121">Relationships</span></span>
<span data-ttu-id="03099-122">Нет</span><span class="sxs-lookup"><span data-stu-id="03099-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03099-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03099-123">JSON Representation</span></span>
<span data-ttu-id="03099-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03099-124">Here is a JSON representation of the resource.</span></span>
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





