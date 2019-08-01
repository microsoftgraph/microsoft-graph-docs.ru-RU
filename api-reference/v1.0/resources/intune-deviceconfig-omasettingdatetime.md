---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71347ecd4a566409d1043c788df70601ffc70a2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028030"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="0655b-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="0655b-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="0655b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0655b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0655b-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0655b-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="0655b-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0655b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0655b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0655b-107">Properties</span></span>
|<span data-ttu-id="0655b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0655b-108">Property</span></span>|<span data-ttu-id="0655b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0655b-109">Type</span></span>|<span data-ttu-id="0655b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0655b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0655b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0655b-111">displayName</span></span>|<span data-ttu-id="0655b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0655b-112">String</span></span>|<span data-ttu-id="0655b-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0655b-113">Display Name.</span></span> <span data-ttu-id="0655b-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0655b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0655b-115">description</span><span class="sxs-lookup"><span data-stu-id="0655b-115">description</span></span>|<span data-ttu-id="0655b-116">String</span><span class="sxs-lookup"><span data-stu-id="0655b-116">String</span></span>|<span data-ttu-id="0655b-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="0655b-117">Description.</span></span> <span data-ttu-id="0655b-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0655b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0655b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="0655b-119">omaUri</span></span>|<span data-ttu-id="0655b-120">String</span><span class="sxs-lookup"><span data-stu-id="0655b-120">String</span></span>|<span data-ttu-id="0655b-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="0655b-121">OMA.</span></span> <span data-ttu-id="0655b-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0655b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0655b-123">value</span><span class="sxs-lookup"><span data-stu-id="0655b-123">value</span></span>|<span data-ttu-id="0655b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0655b-124">DateTimeOffset</span></span>|<span data-ttu-id="0655b-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="0655b-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0655b-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="0655b-126">Relationships</span></span>
<span data-ttu-id="0655b-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0655b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0655b-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0655b-128">JSON Representation</span></span>
<span data-ttu-id="0655b-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0655b-129">Here is a JSON representation of the resource.</span></span>
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



