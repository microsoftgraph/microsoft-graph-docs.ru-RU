---
title: Тип ресурса Девицеманажементаппликабилитирулеоседитион
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0abd5cdde3806b96804f632419e6499be445c16b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332843"
---
# <a name="devicemanagementapplicabilityruleosedition-resource-type"></a><span data-ttu-id="305cf-103">Тип ресурса Девицеманажементаппликабилитирулеоседитион</span><span class="sxs-lookup"><span data-stu-id="305cf-103">deviceManagementApplicabilityRuleOsEdition resource type</span></span>

> <span data-ttu-id="305cf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="305cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="305cf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="305cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="305cf-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="305cf-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="305cf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="305cf-107">Properties</span></span>
|<span data-ttu-id="305cf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="305cf-108">Property</span></span>|<span data-ttu-id="305cf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="305cf-109">Type</span></span>|<span data-ttu-id="305cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="305cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="305cf-111">оседитионтипес</span><span class="sxs-lookup"><span data-stu-id="305cf-111">osEditionTypes</span></span>|<span data-ttu-id="305cf-112">Коллекция [windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)</span><span class="sxs-lookup"><span data-stu-id="305cf-112">[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md) collection</span></span>|<span data-ttu-id="305cf-113">Тип выпуска ОС для правила применимости.</span><span class="sxs-lookup"><span data-stu-id="305cf-113">Applicability rule OS edition type.</span></span>|
|<span data-ttu-id="305cf-114">name</span><span class="sxs-lookup"><span data-stu-id="305cf-114">name</span></span>|<span data-ttu-id="305cf-115">String</span><span class="sxs-lookup"><span data-stu-id="305cf-115">String</span></span>|<span data-ttu-id="305cf-116">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="305cf-116">Name for object.</span></span>|
|<span data-ttu-id="305cf-117">ruleType</span><span class="sxs-lookup"><span data-stu-id="305cf-117">ruleType</span></span>|[<span data-ttu-id="305cf-118">девицеманажементаппликабилитирулетипе</span><span class="sxs-lookup"><span data-stu-id="305cf-118">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="305cf-119">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="305cf-119">Applicability Rule type.</span></span> <span data-ttu-id="305cf-120">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="305cf-120">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="305cf-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="305cf-121">Relationships</span></span>
<span data-ttu-id="305cf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="305cf-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="305cf-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="305cf-123">JSON Representation</span></span>
<span data-ttu-id="305cf-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="305cf-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
  "osEditionTypes": [
    "String"
  ],
  "name": "String",
  "ruleType": "String"
}
```



