---
title: Тип ресурса Девицеманажементаппликабилитирулеосверсион
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c90a026a231998d7cd3ae25ab55ce63c5edb553
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002506"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a><span data-ttu-id="a2d90-103">Тип ресурса Девицеманажементаппликабилитирулеосверсион</span><span class="sxs-lookup"><span data-stu-id="a2d90-103">deviceManagementApplicabilityRuleOsVersion resource type</span></span>

> <span data-ttu-id="a2d90-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2d90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2d90-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2d90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2d90-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a2d90-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a2d90-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2d90-107">Properties</span></span>
|<span data-ttu-id="a2d90-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2d90-108">Property</span></span>|<span data-ttu-id="a2d90-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2d90-109">Type</span></span>|<span data-ttu-id="a2d90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2d90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2d90-111">Миносверсион</span><span class="sxs-lookup"><span data-stu-id="a2d90-111">minOSVersion</span></span>|<span data-ttu-id="a2d90-112">String</span><span class="sxs-lookup"><span data-stu-id="a2d90-112">String</span></span>|<span data-ttu-id="a2d90-113">Минимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="a2d90-113">Min OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="a2d90-114">Максосверсион</span><span class="sxs-lookup"><span data-stu-id="a2d90-114">maxOSVersion</span></span>|<span data-ttu-id="a2d90-115">String</span><span class="sxs-lookup"><span data-stu-id="a2d90-115">String</span></span>|<span data-ttu-id="a2d90-116">Максимальная версия ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="a2d90-116">Max OS version for Applicability Rule.</span></span>|
|<span data-ttu-id="a2d90-117">name</span><span class="sxs-lookup"><span data-stu-id="a2d90-117">name</span></span>|<span data-ttu-id="a2d90-118">String</span><span class="sxs-lookup"><span data-stu-id="a2d90-118">String</span></span>|<span data-ttu-id="a2d90-119">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="a2d90-119">Name for object.</span></span>|
|<span data-ttu-id="a2d90-120">ruleType</span><span class="sxs-lookup"><span data-stu-id="a2d90-120">ruleType</span></span>|[<span data-ttu-id="a2d90-121">Девицеманажементаппликабилитирулетипе</span><span class="sxs-lookup"><span data-stu-id="a2d90-121">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="a2d90-122">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="a2d90-122">Applicability Rule type.</span></span> <span data-ttu-id="a2d90-123">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="a2d90-123">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2d90-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="a2d90-124">Relationships</span></span>
<span data-ttu-id="a2d90-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a2d90-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2d90-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2d90-126">JSON Representation</span></span>
<span data-ttu-id="a2d90-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2d90-127">Here is a JSON representation of the resource.</span></span>
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





