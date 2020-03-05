---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c86d863d3adf85a04666845c8e4fbc223c7c263
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493890"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="eee78-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="eee78-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="eee78-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eee78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eee78-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eee78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eee78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eee78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eee78-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="eee78-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="eee78-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eee78-108">Properties</span></span>
|<span data-ttu-id="eee78-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eee78-109">Property</span></span>|<span data-ttu-id="eee78-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eee78-110">Type</span></span>|<span data-ttu-id="eee78-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eee78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee78-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="eee78-112">appConfigKey</span></span>|<span data-ttu-id="eee78-113">String</span><span class="sxs-lookup"><span data-stu-id="eee78-113">String</span></span>|<span data-ttu-id="eee78-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="eee78-114">app configuration key.</span></span>|
|<span data-ttu-id="eee78-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="eee78-115">appConfigKeyType</span></span>|[<span data-ttu-id="eee78-116">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="eee78-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="eee78-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="eee78-117">app configuration key type.</span></span> <span data-ttu-id="eee78-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="eee78-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="eee78-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="eee78-119">appConfigKeyValue</span></span>|<span data-ttu-id="eee78-120">Строка</span><span class="sxs-lookup"><span data-stu-id="eee78-120">String</span></span>|<span data-ttu-id="eee78-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="eee78-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eee78-122">Связи</span><span class="sxs-lookup"><span data-stu-id="eee78-122">Relationships</span></span>
<span data-ttu-id="eee78-123">Нет</span><span class="sxs-lookup"><span data-stu-id="eee78-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eee78-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eee78-124">JSON Representation</span></span>
<span data-ttu-id="eee78-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eee78-125">Here is a JSON representation of the resource.</span></span>
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



