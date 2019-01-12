---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb7b503ff14e6499342fafc2d0cf5ab8e670138
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960338"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="e2049-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="e2049-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="e2049-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2049-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2049-105">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2049-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="e2049-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2049-106">Properties</span></span>
|<span data-ttu-id="e2049-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2049-107">Property</span></span>|<span data-ttu-id="e2049-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2049-108">Type</span></span>|<span data-ttu-id="e2049-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2049-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2049-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="e2049-110">appConfigKey</span></span>|<span data-ttu-id="e2049-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e2049-111">String</span></span>|<span data-ttu-id="e2049-112">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2049-112">app configuration key.</span></span>|
|<span data-ttu-id="e2049-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e2049-113">appConfigKeyType</span></span>|[<span data-ttu-id="e2049-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e2049-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="e2049-115">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2049-115">app configuration key type.</span></span> <span data-ttu-id="e2049-116">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="e2049-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="e2049-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="e2049-117">appConfigKeyValue</span></span>|<span data-ttu-id="e2049-118">Строка</span><span class="sxs-lookup"><span data-stu-id="e2049-118">String</span></span>|<span data-ttu-id="e2049-119">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="e2049-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2049-120">Связи</span><span class="sxs-lookup"><span data-stu-id="e2049-120">Relationships</span></span>
<span data-ttu-id="e2049-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e2049-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2049-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2049-122">JSON Representation</span></span>
<span data-ttu-id="e2049-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2049-123">Here is a JSON representation of the resource.</span></span>
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



