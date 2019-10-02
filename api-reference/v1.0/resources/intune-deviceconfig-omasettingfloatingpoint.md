---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2f397d309f2199458595e3ed7d5cd4a204a1874
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359931"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="240ec-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="240ec-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="240ec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="240ec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="240ec-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="240ec-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="240ec-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="240ec-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="240ec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="240ec-107">Properties</span></span>
|<span data-ttu-id="240ec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="240ec-108">Property</span></span>|<span data-ttu-id="240ec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="240ec-109">Type</span></span>|<span data-ttu-id="240ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="240ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="240ec-111">displayName</span><span class="sxs-lookup"><span data-stu-id="240ec-111">displayName</span></span>|<span data-ttu-id="240ec-112">Строка</span><span class="sxs-lookup"><span data-stu-id="240ec-112">String</span></span>|<span data-ttu-id="240ec-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="240ec-113">Display Name.</span></span> <span data-ttu-id="240ec-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="240ec-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="240ec-115">description</span><span class="sxs-lookup"><span data-stu-id="240ec-115">description</span></span>|<span data-ttu-id="240ec-116">String</span><span class="sxs-lookup"><span data-stu-id="240ec-116">String</span></span>|<span data-ttu-id="240ec-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="240ec-117">Description.</span></span> <span data-ttu-id="240ec-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="240ec-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="240ec-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="240ec-119">omaUri</span></span>|<span data-ttu-id="240ec-120">String</span><span class="sxs-lookup"><span data-stu-id="240ec-120">String</span></span>|<span data-ttu-id="240ec-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="240ec-121">OMA.</span></span> <span data-ttu-id="240ec-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="240ec-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="240ec-123">value</span><span class="sxs-lookup"><span data-stu-id="240ec-123">value</span></span>|<span data-ttu-id="240ec-124">Single</span><span class="sxs-lookup"><span data-stu-id="240ec-124">Single</span></span>|<span data-ttu-id="240ec-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="240ec-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="240ec-126">Связи</span><span class="sxs-lookup"><span data-stu-id="240ec-126">Relationships</span></span>
<span data-ttu-id="240ec-127">Нет</span><span class="sxs-lookup"><span data-stu-id="240ec-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="240ec-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="240ec-128">JSON Representation</span></span>
<span data-ttu-id="240ec-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="240ec-129">Here is a JSON representation of the resource.</span></span>
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




