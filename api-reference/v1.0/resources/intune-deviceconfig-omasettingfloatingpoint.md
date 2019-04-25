---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568999"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="0dc97-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="0dc97-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="0dc97-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0dc97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dc97-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0dc97-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="0dc97-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0dc97-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0dc97-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0dc97-107">Properties</span></span>
|<span data-ttu-id="0dc97-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0dc97-108">Property</span></span>|<span data-ttu-id="0dc97-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0dc97-109">Type</span></span>|<span data-ttu-id="0dc97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0dc97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dc97-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0dc97-111">displayName</span></span>|<span data-ttu-id="0dc97-112">String</span><span class="sxs-lookup"><span data-stu-id="0dc97-112">String</span></span>|<span data-ttu-id="0dc97-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0dc97-113">Display Name.</span></span> <span data-ttu-id="0dc97-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0dc97-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0dc97-115">description</span><span class="sxs-lookup"><span data-stu-id="0dc97-115">description</span></span>|<span data-ttu-id="0dc97-116">String</span><span class="sxs-lookup"><span data-stu-id="0dc97-116">String</span></span>|<span data-ttu-id="0dc97-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="0dc97-117">Description.</span></span> <span data-ttu-id="0dc97-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0dc97-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0dc97-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0dc97-119">omaUri</span></span>|<span data-ttu-id="0dc97-120">String</span><span class="sxs-lookup"><span data-stu-id="0dc97-120">String</span></span>|<span data-ttu-id="0dc97-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0dc97-121">OMA.</span></span> <span data-ttu-id="0dc97-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0dc97-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0dc97-123">value</span><span class="sxs-lookup"><span data-stu-id="0dc97-123">value</span></span>|<span data-ttu-id="0dc97-124">Single</span><span class="sxs-lookup"><span data-stu-id="0dc97-124">Single</span></span>|<span data-ttu-id="0dc97-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="0dc97-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dc97-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="0dc97-126">Relationships</span></span>
<span data-ttu-id="0dc97-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0dc97-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dc97-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0dc97-128">JSON Representation</span></span>
<span data-ttu-id="0dc97-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0dc97-129">Here is a JSON representation of the resource.</span></span>
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



