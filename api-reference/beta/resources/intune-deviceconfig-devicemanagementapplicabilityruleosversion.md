---
title: Тип ресурса Девицеманажементаппликабилитирулеосверсион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a8195bd67cf64d1875b795c3609cf04f9c13b31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031699"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="b92e0-103">Тип ресурса Девицеманажементаппликабилитирулеосверсион</span><span class="sxs-lookup"><span data-stu-id="b92e0-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

<span data-ttu-id="b92e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b92e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b92e0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b92e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b92e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b92e0-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b92e0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b92e0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b92e0-108">Properties</span></span>
|<span data-ttu-id="b92e0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b92e0-109">Property</span></span>|<span data-ttu-id="b92e0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b92e0-110">Type</span></span>|<span data-ttu-id="b92e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b92e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b92e0-112">миносверсион</span><span class="sxs-lookup"><span data-stu-id="b92e0-112">minOSVersion</span></span>|<span data-ttu-id="b92e0-113">String</span><span class="sxs-lookup"><span data-stu-id="b92e0-113">String</span></span>|<span data-ttu-id="b92e0-114">Минимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="b92e0-114">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="b92e0-115">максосверсион</span><span class="sxs-lookup"><span data-stu-id="b92e0-115">maxOSVersion</span></span>|<span data-ttu-id="b92e0-116">String</span><span class="sxs-lookup"><span data-stu-id="b92e0-116">String</span></span>|<span data-ttu-id="b92e0-117">Максимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="b92e0-117">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="b92e0-118">name</span><span class="sxs-lookup"><span data-stu-id="b92e0-118">name</span></span>|<span data-ttu-id="b92e0-119">String</span><span class="sxs-lookup"><span data-stu-id="b92e0-119">String</span></span>|<span data-ttu-id="b92e0-120">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="b92e0-120">Name for object.</span></span>|
|<span data-ttu-id="b92e0-121">ruleType</span><span class="sxs-lookup"><span data-stu-id="b92e0-121">ruleType</span></span>|[<span data-ttu-id="b92e0-122">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="b92e0-122">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="b92e0-123">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="b92e0-123">Applicability Rule type.</span></span> <span data-ttu-id="b92e0-124">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="b92e0-124">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b92e0-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="b92e0-125">Relationships</span></span>
<span data-ttu-id="b92e0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b92e0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b92e0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b92e0-127">JSON Representation</span></span>
<span data-ttu-id="b92e0-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b92e0-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```






