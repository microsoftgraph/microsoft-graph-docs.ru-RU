---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc552bc2dcaf04990999c9414d2723284a568f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045469"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="2d268-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="2d268-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="2d268-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d268-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d268-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d268-106">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2d268-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="2d268-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d268-107">Properties</span></span>
|<span data-ttu-id="2d268-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d268-108">Property</span></span>|<span data-ttu-id="2d268-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2d268-109">Type</span></span>|<span data-ttu-id="2d268-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d268-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d268-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="2d268-111">appConfigKey</span></span>|<span data-ttu-id="2d268-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2d268-112">String</span></span>|<span data-ttu-id="2d268-113">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2d268-113">app configuration key.</span></span>|
|<span data-ttu-id="2d268-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2d268-114">appConfigKeyType</span></span>|[<span data-ttu-id="2d268-115">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="2d268-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="2d268-116">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2d268-116">app configuration key type.</span></span> <span data-ttu-id="2d268-117">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="2d268-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="2d268-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="2d268-118">appConfigKeyValue</span></span>|<span data-ttu-id="2d268-119">Строка</span><span class="sxs-lookup"><span data-stu-id="2d268-119">String</span></span>|<span data-ttu-id="2d268-120">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2d268-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d268-121">Связи</span><span class="sxs-lookup"><span data-stu-id="2d268-121">Relationships</span></span>
<span data-ttu-id="2d268-122">Нет</span><span class="sxs-lookup"><span data-stu-id="2d268-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d268-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d268-123">JSON Representation</span></span>
<span data-ttu-id="2d268-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d268-124">Here is a JSON representation of the resource.</span></span>
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









