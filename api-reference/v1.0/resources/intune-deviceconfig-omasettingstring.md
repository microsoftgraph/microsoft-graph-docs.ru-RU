---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79261fe777d6251ba3c08d87d5d5a3d26ee83b53
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359917"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="acb91-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="acb91-103">omaSettingString resource type</span></span>

> <span data-ttu-id="acb91-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acb91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acb91-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="acb91-105">OMA Settings String definition.</span></span>


<span data-ttu-id="acb91-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="acb91-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="acb91-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="acb91-107">Properties</span></span>
|<span data-ttu-id="acb91-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="acb91-108">Property</span></span>|<span data-ttu-id="acb91-109">Тип</span><span class="sxs-lookup"><span data-stu-id="acb91-109">Type</span></span>|<span data-ttu-id="acb91-110">Описание</span><span class="sxs-lookup"><span data-stu-id="acb91-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acb91-111">displayName</span><span class="sxs-lookup"><span data-stu-id="acb91-111">displayName</span></span>|<span data-ttu-id="acb91-112">Строка</span><span class="sxs-lookup"><span data-stu-id="acb91-112">String</span></span>|<span data-ttu-id="acb91-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="acb91-113">Display Name.</span></span> <span data-ttu-id="acb91-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="acb91-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="acb91-115">description</span><span class="sxs-lookup"><span data-stu-id="acb91-115">description</span></span>|<span data-ttu-id="acb91-116">String</span><span class="sxs-lookup"><span data-stu-id="acb91-116">String</span></span>|<span data-ttu-id="acb91-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="acb91-117">Description.</span></span> <span data-ttu-id="acb91-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="acb91-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="acb91-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="acb91-119">omaUri</span></span>|<span data-ttu-id="acb91-120">String</span><span class="sxs-lookup"><span data-stu-id="acb91-120">String</span></span>|<span data-ttu-id="acb91-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="acb91-121">OMA.</span></span> <span data-ttu-id="acb91-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="acb91-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="acb91-123">value</span><span class="sxs-lookup"><span data-stu-id="acb91-123">value</span></span>|<span data-ttu-id="acb91-124">Строка</span><span class="sxs-lookup"><span data-stu-id="acb91-124">String</span></span>|<span data-ttu-id="acb91-125">Значение</span><span class="sxs-lookup"><span data-stu-id="acb91-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acb91-126">Связи</span><span class="sxs-lookup"><span data-stu-id="acb91-126">Relationships</span></span>
<span data-ttu-id="acb91-127">Нет</span><span class="sxs-lookup"><span data-stu-id="acb91-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acb91-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acb91-128">JSON Representation</span></span>
<span data-ttu-id="acb91-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acb91-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```




