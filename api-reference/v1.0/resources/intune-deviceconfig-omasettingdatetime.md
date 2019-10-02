---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4405f8446ceb76dbdd5b4c9df1407ee14861a3b8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360799"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="2b367-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="2b367-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="2b367-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b367-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b367-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="2b367-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="2b367-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2b367-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2b367-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b367-107">Properties</span></span>
|<span data-ttu-id="2b367-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b367-108">Property</span></span>|<span data-ttu-id="2b367-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b367-109">Type</span></span>|<span data-ttu-id="2b367-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b367-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b367-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2b367-111">displayName</span></span>|<span data-ttu-id="2b367-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2b367-112">String</span></span>|<span data-ttu-id="2b367-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2b367-113">Display Name.</span></span> <span data-ttu-id="2b367-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2b367-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2b367-115">description</span><span class="sxs-lookup"><span data-stu-id="2b367-115">description</span></span>|<span data-ttu-id="2b367-116">String</span><span class="sxs-lookup"><span data-stu-id="2b367-116">String</span></span>|<span data-ttu-id="2b367-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="2b367-117">Description.</span></span> <span data-ttu-id="2b367-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2b367-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2b367-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="2b367-119">omaUri</span></span>|<span data-ttu-id="2b367-120">String</span><span class="sxs-lookup"><span data-stu-id="2b367-120">String</span></span>|<span data-ttu-id="2b367-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="2b367-121">OMA.</span></span> <span data-ttu-id="2b367-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2b367-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2b367-123">value</span><span class="sxs-lookup"><span data-stu-id="2b367-123">value</span></span>|<span data-ttu-id="2b367-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b367-124">DateTimeOffset</span></span>|<span data-ttu-id="2b367-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="2b367-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b367-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2b367-126">Relationships</span></span>
<span data-ttu-id="2b367-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2b367-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b367-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b367-128">JSON Representation</span></span>
<span data-ttu-id="2b367-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b367-129">Here is a JSON representation of the resource.</span></span>
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




