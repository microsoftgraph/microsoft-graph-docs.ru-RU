---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a237f36a209e2fa1d552c8f50207770429a0c53
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789691"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="87ecc-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="87ecc-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="87ecc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ecc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87ecc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87ecc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ecc-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="87ecc-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="87ecc-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="87ecc-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="87ecc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="87ecc-108">Properties</span></span>
|<span data-ttu-id="87ecc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="87ecc-109">Property</span></span>|<span data-ttu-id="87ecc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="87ecc-110">Type</span></span>|<span data-ttu-id="87ecc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87ecc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ecc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="87ecc-112">displayName</span></span>|<span data-ttu-id="87ecc-113">String</span><span class="sxs-lookup"><span data-stu-id="87ecc-113">String</span></span>|<span data-ttu-id="87ecc-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="87ecc-114">Display Name.</span></span> <span data-ttu-id="87ecc-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="87ecc-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="87ecc-116">description</span><span class="sxs-lookup"><span data-stu-id="87ecc-116">description</span></span>|<span data-ttu-id="87ecc-117">String</span><span class="sxs-lookup"><span data-stu-id="87ecc-117">String</span></span>|<span data-ttu-id="87ecc-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="87ecc-118">Description.</span></span> <span data-ttu-id="87ecc-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="87ecc-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="87ecc-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="87ecc-120">omaUri</span></span>|<span data-ttu-id="87ecc-121">String</span><span class="sxs-lookup"><span data-stu-id="87ecc-121">String</span></span>|<span data-ttu-id="87ecc-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="87ecc-122">OMA.</span></span> <span data-ttu-id="87ecc-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="87ecc-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="87ecc-124">value</span><span class="sxs-lookup"><span data-stu-id="87ecc-124">value</span></span>|<span data-ttu-id="87ecc-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87ecc-125">DateTimeOffset</span></span>|<span data-ttu-id="87ecc-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="87ecc-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87ecc-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="87ecc-127">Relationships</span></span>
<span data-ttu-id="87ecc-128">Нет</span><span class="sxs-lookup"><span data-stu-id="87ecc-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87ecc-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87ecc-129">JSON Representation</span></span>
<span data-ttu-id="87ecc-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87ecc-130">Here is a JSON representation of the resource.</span></span>
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





