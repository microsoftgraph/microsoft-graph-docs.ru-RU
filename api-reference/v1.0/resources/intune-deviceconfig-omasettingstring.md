---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259915"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="f3974-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="f3974-103">omaSettingString resource type</span></span>

> <span data-ttu-id="f3974-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3974-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3974-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="f3974-105">OMA Settings String definition.</span></span>


<span data-ttu-id="f3974-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3974-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3974-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3974-107">Properties</span></span>
|<span data-ttu-id="f3974-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3974-108">Property</span></span>|<span data-ttu-id="f3974-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f3974-109">Type</span></span>|<span data-ttu-id="f3974-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f3974-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3974-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f3974-111">displayName</span></span>|<span data-ttu-id="f3974-112">String</span><span class="sxs-lookup"><span data-stu-id="f3974-112">String</span></span>|<span data-ttu-id="f3974-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f3974-113">Display Name.</span></span> <span data-ttu-id="f3974-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3974-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3974-115">description</span><span class="sxs-lookup"><span data-stu-id="f3974-115">description</span></span>|<span data-ttu-id="f3974-116">String</span><span class="sxs-lookup"><span data-stu-id="f3974-116">String</span></span>|<span data-ttu-id="f3974-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="f3974-117">Description.</span></span> <span data-ttu-id="f3974-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3974-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3974-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f3974-119">omaUri</span></span>|<span data-ttu-id="f3974-120">String</span><span class="sxs-lookup"><span data-stu-id="f3974-120">String</span></span>|<span data-ttu-id="f3974-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="f3974-121">OMA.</span></span> <span data-ttu-id="f3974-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3974-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3974-123">value</span><span class="sxs-lookup"><span data-stu-id="f3974-123">value</span></span>|<span data-ttu-id="f3974-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f3974-124">String</span></span>|<span data-ttu-id="f3974-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f3974-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3974-126">Связи</span><span class="sxs-lookup"><span data-stu-id="f3974-126">Relationships</span></span>
<span data-ttu-id="f3974-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f3974-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3974-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3974-128">JSON Representation</span></span>
<span data-ttu-id="f3974-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3974-129">Here is a JSON representation of the resource.</span></span>
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



