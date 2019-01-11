---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 900a16544b0166263b7d40c428c2c4cbaf5a0bb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830424"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="9a985-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="9a985-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="9a985-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9a985-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a985-105">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9a985-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="9a985-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a985-106">Properties</span></span>
|<span data-ttu-id="9a985-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a985-107">Property</span></span>|<span data-ttu-id="9a985-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a985-108">Type</span></span>|<span data-ttu-id="9a985-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a985-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a985-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="9a985-110">appConfigKey</span></span>|<span data-ttu-id="9a985-111">Строка</span><span class="sxs-lookup"><span data-stu-id="9a985-111">String</span></span>|<span data-ttu-id="9a985-112">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9a985-112">app configuration key.</span></span>|
|<span data-ttu-id="9a985-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9a985-113">appConfigKeyType</span></span>|[<span data-ttu-id="9a985-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="9a985-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="9a985-115">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9a985-115">app configuration key type.</span></span> <span data-ttu-id="9a985-116">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="9a985-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="9a985-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="9a985-117">appConfigKeyValue</span></span>|<span data-ttu-id="9a985-118">Строка</span><span class="sxs-lookup"><span data-stu-id="9a985-118">String</span></span>|<span data-ttu-id="9a985-119">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9a985-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a985-120">Связи</span><span class="sxs-lookup"><span data-stu-id="9a985-120">Relationships</span></span>
<span data-ttu-id="9a985-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9a985-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9a985-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a985-122">JSON Representation</span></span>
<span data-ttu-id="9a985-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a985-123">Here is a JSON representation of the resource.</span></span>
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



