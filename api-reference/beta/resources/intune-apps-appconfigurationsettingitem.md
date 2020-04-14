---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e71ad9bddd6595f6057463aa01116727e368c46
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459136"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="00931-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="00931-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="00931-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00931-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00931-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00931-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00931-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00931-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00931-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="00931-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="00931-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00931-108">Properties</span></span>
|<span data-ttu-id="00931-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00931-109">Property</span></span>|<span data-ttu-id="00931-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00931-110">Type</span></span>|<span data-ttu-id="00931-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00931-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00931-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="00931-112">appConfigKey</span></span>|<span data-ttu-id="00931-113">String</span><span class="sxs-lookup"><span data-stu-id="00931-113">String</span></span>|<span data-ttu-id="00931-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="00931-114">app configuration key.</span></span>|
|<span data-ttu-id="00931-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="00931-115">appConfigKeyType</span></span>|[<span data-ttu-id="00931-116">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="00931-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="00931-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="00931-117">app configuration key type.</span></span> <span data-ttu-id="00931-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="00931-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="00931-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="00931-119">appConfigKeyValue</span></span>|<span data-ttu-id="00931-120">Строка</span><span class="sxs-lookup"><span data-stu-id="00931-120">String</span></span>|<span data-ttu-id="00931-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="00931-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00931-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="00931-122">Relationships</span></span>
<span data-ttu-id="00931-123">Нет</span><span class="sxs-lookup"><span data-stu-id="00931-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00931-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00931-124">JSON Representation</span></span>
<span data-ttu-id="00931-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00931-125">Here is a JSON representation of the resource.</span></span>
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



