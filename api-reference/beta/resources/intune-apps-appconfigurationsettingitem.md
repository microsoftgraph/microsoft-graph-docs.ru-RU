---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b4d76284c5fbc099a24a4c848613302e0fd630f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727528"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="b80f5-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="b80f5-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="b80f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b80f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b80f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b80f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b80f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b80f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b80f5-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b80f5-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="b80f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b80f5-108">Properties</span></span>
|<span data-ttu-id="b80f5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b80f5-109">Property</span></span>|<span data-ttu-id="b80f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b80f5-110">Type</span></span>|<span data-ttu-id="b80f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b80f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b80f5-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="b80f5-112">appConfigKey</span></span>|<span data-ttu-id="b80f5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b80f5-113">String</span></span>|<span data-ttu-id="b80f5-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b80f5-114">app configuration key.</span></span>|
|<span data-ttu-id="b80f5-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="b80f5-115">appConfigKeyType</span></span>|[<span data-ttu-id="b80f5-116">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="b80f5-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="b80f5-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b80f5-117">app configuration key type.</span></span> <span data-ttu-id="b80f5-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="b80f5-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="b80f5-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="b80f5-119">appConfigKeyValue</span></span>|<span data-ttu-id="b80f5-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b80f5-120">String</span></span>|<span data-ttu-id="b80f5-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b80f5-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b80f5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="b80f5-122">Relationships</span></span>
<span data-ttu-id="b80f5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b80f5-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b80f5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b80f5-124">JSON Representation</span></span>
<span data-ttu-id="b80f5-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b80f5-125">Here is a JSON representation of the resource.</span></span>
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





