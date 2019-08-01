---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30802cc391958fabec4540fc3256f7c67ec094c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031306"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="3c43f-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="3c43f-103">omaSettingString resource type</span></span>

> <span data-ttu-id="3c43f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c43f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c43f-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="3c43f-105">OMA Settings String definition.</span></span>


<span data-ttu-id="3c43f-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3c43f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3c43f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c43f-107">Properties</span></span>
|<span data-ttu-id="3c43f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c43f-108">Property</span></span>|<span data-ttu-id="3c43f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c43f-109">Type</span></span>|<span data-ttu-id="3c43f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c43f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c43f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3c43f-111">displayName</span></span>|<span data-ttu-id="3c43f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="3c43f-112">String</span></span>|<span data-ttu-id="3c43f-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3c43f-113">Display Name.</span></span> <span data-ttu-id="3c43f-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3c43f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3c43f-115">description</span><span class="sxs-lookup"><span data-stu-id="3c43f-115">description</span></span>|<span data-ttu-id="3c43f-116">String</span><span class="sxs-lookup"><span data-stu-id="3c43f-116">String</span></span>|<span data-ttu-id="3c43f-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="3c43f-117">Description.</span></span> <span data-ttu-id="3c43f-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3c43f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3c43f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="3c43f-119">omaUri</span></span>|<span data-ttu-id="3c43f-120">String</span><span class="sxs-lookup"><span data-stu-id="3c43f-120">String</span></span>|<span data-ttu-id="3c43f-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="3c43f-121">OMA.</span></span> <span data-ttu-id="3c43f-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3c43f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3c43f-123">value</span><span class="sxs-lookup"><span data-stu-id="3c43f-123">value</span></span>|<span data-ttu-id="3c43f-124">Строка</span><span class="sxs-lookup"><span data-stu-id="3c43f-124">String</span></span>|<span data-ttu-id="3c43f-125">Значение</span><span class="sxs-lookup"><span data-stu-id="3c43f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c43f-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c43f-126">Relationships</span></span>
<span data-ttu-id="3c43f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="3c43f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c43f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c43f-128">JSON Representation</span></span>
<span data-ttu-id="3c43f-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c43f-129">Here is a JSON representation of the resource.</span></span>
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



