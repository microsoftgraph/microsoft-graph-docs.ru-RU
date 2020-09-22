---
title: Тип ресурса appConfigurationSettingItem
description: Содержит свойства для элемента параметра конфигурации приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e2ec0f05b7bb40d97458a7d9fa452edc9124451
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003999"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="02c85-103">Тип ресурса appConfigurationSettingItem</span><span class="sxs-lookup"><span data-stu-id="02c85-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="02c85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02c85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02c85-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02c85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02c85-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02c85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02c85-107">Содержит свойства для элемента параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="02c85-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="02c85-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="02c85-108">Properties</span></span>
|<span data-ttu-id="02c85-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c85-109">Property</span></span>|<span data-ttu-id="02c85-110">Тип</span><span class="sxs-lookup"><span data-stu-id="02c85-110">Type</span></span>|<span data-ttu-id="02c85-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02c85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02c85-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="02c85-112">appConfigKey</span></span>|<span data-ttu-id="02c85-113">Строка</span><span class="sxs-lookup"><span data-stu-id="02c85-113">String</span></span>|<span data-ttu-id="02c85-114">Ключ конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="02c85-114">app configuration key.</span></span>|
|<span data-ttu-id="02c85-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="02c85-115">appConfigKeyType</span></span>|[<span data-ttu-id="02c85-116">мдмаппконфигкэйтипе</span><span class="sxs-lookup"><span data-stu-id="02c85-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="02c85-117">Тип ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="02c85-117">app configuration key type.</span></span> <span data-ttu-id="02c85-118">Возможные значения: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="02c85-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="02c85-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="02c85-119">appConfigKeyValue</span></span>|<span data-ttu-id="02c85-120">Строка</span><span class="sxs-lookup"><span data-stu-id="02c85-120">String</span></span>|<span data-ttu-id="02c85-121">Значение ключа конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="02c85-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02c85-122">Связи</span><span class="sxs-lookup"><span data-stu-id="02c85-122">Relationships</span></span>
<span data-ttu-id="02c85-123">Нет</span><span class="sxs-lookup"><span data-stu-id="02c85-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02c85-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02c85-124">JSON Representation</span></span>
<span data-ttu-id="02c85-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02c85-125">Here is a JSON representation of the resource.</span></span>
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






