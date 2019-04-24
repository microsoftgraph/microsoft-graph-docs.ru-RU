---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585400"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d2969-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="d2969-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="d2969-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2969-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2969-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d2969-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="d2969-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2969-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2969-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2969-107">Properties</span></span>
|<span data-ttu-id="d2969-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2969-108">Property</span></span>|<span data-ttu-id="d2969-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2969-109">Type</span></span>|<span data-ttu-id="d2969-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2969-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2969-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d2969-111">displayName</span></span>|<span data-ttu-id="d2969-112">String</span><span class="sxs-lookup"><span data-stu-id="d2969-112">String</span></span>|<span data-ttu-id="d2969-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d2969-113">Display Name.</span></span> <span data-ttu-id="d2969-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2969-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2969-115">description</span><span class="sxs-lookup"><span data-stu-id="d2969-115">description</span></span>|<span data-ttu-id="d2969-116">String</span><span class="sxs-lookup"><span data-stu-id="d2969-116">String</span></span>|<span data-ttu-id="d2969-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="d2969-117">Description.</span></span> <span data-ttu-id="d2969-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2969-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2969-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d2969-119">omaUri</span></span>|<span data-ttu-id="d2969-120">String</span><span class="sxs-lookup"><span data-stu-id="d2969-120">String</span></span>|<span data-ttu-id="d2969-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="d2969-121">OMA.</span></span> <span data-ttu-id="d2969-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d2969-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d2969-123">value</span><span class="sxs-lookup"><span data-stu-id="d2969-123">value</span></span>|<span data-ttu-id="d2969-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2969-124">DateTimeOffset</span></span>|<span data-ttu-id="d2969-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="d2969-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2969-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2969-126">Relationships</span></span>
<span data-ttu-id="d2969-127">Нет</span><span class="sxs-lookup"><span data-stu-id="d2969-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2969-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2969-128">JSON Representation</span></span>
<span data-ttu-id="d2969-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2969-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



