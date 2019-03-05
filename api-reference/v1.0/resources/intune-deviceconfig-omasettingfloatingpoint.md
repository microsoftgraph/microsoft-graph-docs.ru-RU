---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255033"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="0e482-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="0e482-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="0e482-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e482-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e482-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0e482-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="0e482-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e482-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e482-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e482-107">Properties</span></span>
|<span data-ttu-id="0e482-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e482-108">Property</span></span>|<span data-ttu-id="0e482-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0e482-109">Type</span></span>|<span data-ttu-id="0e482-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e482-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e482-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0e482-111">displayName</span></span>|<span data-ttu-id="0e482-112">String</span><span class="sxs-lookup"><span data-stu-id="0e482-112">String</span></span>|<span data-ttu-id="0e482-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0e482-113">Display Name.</span></span> <span data-ttu-id="0e482-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e482-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e482-115">description</span><span class="sxs-lookup"><span data-stu-id="0e482-115">description</span></span>|<span data-ttu-id="0e482-116">String</span><span class="sxs-lookup"><span data-stu-id="0e482-116">String</span></span>|<span data-ttu-id="0e482-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="0e482-117">Description.</span></span> <span data-ttu-id="0e482-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e482-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e482-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0e482-119">omaUri</span></span>|<span data-ttu-id="0e482-120">String</span><span class="sxs-lookup"><span data-stu-id="0e482-120">String</span></span>|<span data-ttu-id="0e482-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0e482-121">OMA.</span></span> <span data-ttu-id="0e482-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0e482-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0e482-123">value</span><span class="sxs-lookup"><span data-stu-id="0e482-123">value</span></span>|<span data-ttu-id="0e482-124">Single</span><span class="sxs-lookup"><span data-stu-id="0e482-124">Single</span></span>|<span data-ttu-id="0e482-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="0e482-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e482-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0e482-126">Relationships</span></span>
<span data-ttu-id="0e482-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0e482-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e482-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e482-128">JSON Representation</span></span>
<span data-ttu-id="0e482-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e482-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



