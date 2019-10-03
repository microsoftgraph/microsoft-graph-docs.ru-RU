---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a93824eec0df18984809b0580c4a1dcb5caec55
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366575"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="4b539-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="4b539-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="4b539-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b539-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b539-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="4b539-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="4b539-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b539-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b539-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b539-107">Properties</span></span>
|<span data-ttu-id="4b539-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b539-108">Property</span></span>|<span data-ttu-id="4b539-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b539-109">Type</span></span>|<span data-ttu-id="4b539-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b539-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b539-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4b539-111">displayName</span></span>|<span data-ttu-id="4b539-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4b539-112">String</span></span>|<span data-ttu-id="4b539-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4b539-113">Display Name.</span></span> <span data-ttu-id="4b539-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b539-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b539-115">description</span><span class="sxs-lookup"><span data-stu-id="4b539-115">description</span></span>|<span data-ttu-id="4b539-116">String</span><span class="sxs-lookup"><span data-stu-id="4b539-116">String</span></span>|<span data-ttu-id="4b539-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="4b539-117">Description.</span></span> <span data-ttu-id="4b539-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b539-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b539-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4b539-119">omaUri</span></span>|<span data-ttu-id="4b539-120">String</span><span class="sxs-lookup"><span data-stu-id="4b539-120">String</span></span>|<span data-ttu-id="4b539-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="4b539-121">OMA.</span></span> <span data-ttu-id="4b539-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b539-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b539-123">value</span><span class="sxs-lookup"><span data-stu-id="4b539-123">value</span></span>|<span data-ttu-id="4b539-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b539-124">Boolean</span></span>|<span data-ttu-id="4b539-125">Значение</span><span class="sxs-lookup"><span data-stu-id="4b539-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b539-126">Связи</span><span class="sxs-lookup"><span data-stu-id="4b539-126">Relationships</span></span>
<span data-ttu-id="4b539-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4b539-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b539-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b539-128">JSON Representation</span></span>
<span data-ttu-id="4b539-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b539-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




