---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85eeeff4cc9ac897416e587aa5d26be79b59bb59
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359903"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="c2dcb-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="c2dcb-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="c2dcb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2dcb-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="c2dcb-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2dcb-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2dcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2dcb-107">Properties</span></span>
|<span data-ttu-id="c2dcb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2dcb-108">Property</span></span>|<span data-ttu-id="c2dcb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2dcb-109">Type</span></span>|<span data-ttu-id="c2dcb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2dcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2dcb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c2dcb-111">displayName</span></span>|<span data-ttu-id="c2dcb-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c2dcb-112">String</span></span>|<span data-ttu-id="c2dcb-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-113">Display Name.</span></span> <span data-ttu-id="c2dcb-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2dcb-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2dcb-115">description</span><span class="sxs-lookup"><span data-stu-id="c2dcb-115">description</span></span>|<span data-ttu-id="c2dcb-116">String</span><span class="sxs-lookup"><span data-stu-id="c2dcb-116">String</span></span>|<span data-ttu-id="c2dcb-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-117">Description.</span></span> <span data-ttu-id="c2dcb-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2dcb-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2dcb-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="c2dcb-119">omaUri</span></span>|<span data-ttu-id="c2dcb-120">String</span><span class="sxs-lookup"><span data-stu-id="c2dcb-120">String</span></span>|<span data-ttu-id="c2dcb-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-121">OMA.</span></span> <span data-ttu-id="c2dcb-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2dcb-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2dcb-123">value</span><span class="sxs-lookup"><span data-stu-id="c2dcb-123">value</span></span>|<span data-ttu-id="c2dcb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="c2dcb-124">Int32</span></span>|<span data-ttu-id="c2dcb-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2dcb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="c2dcb-126">Relationships</span></span>
<span data-ttu-id="c2dcb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c2dcb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2dcb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2dcb-128">JSON Representation</span></span>
<span data-ttu-id="c2dcb-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2dcb-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```




