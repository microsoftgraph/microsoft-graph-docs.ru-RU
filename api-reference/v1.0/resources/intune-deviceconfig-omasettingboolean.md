---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256394"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="ea971-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="ea971-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="ea971-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea971-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea971-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="ea971-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="ea971-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ea971-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea971-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea971-107">Properties</span></span>
|<span data-ttu-id="ea971-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea971-108">Property</span></span>|<span data-ttu-id="ea971-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ea971-109">Type</span></span>|<span data-ttu-id="ea971-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ea971-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea971-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ea971-111">displayName</span></span>|<span data-ttu-id="ea971-112">String</span><span class="sxs-lookup"><span data-stu-id="ea971-112">String</span></span>|<span data-ttu-id="ea971-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ea971-113">Display Name.</span></span> <span data-ttu-id="ea971-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ea971-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ea971-115">description</span><span class="sxs-lookup"><span data-stu-id="ea971-115">description</span></span>|<span data-ttu-id="ea971-116">String</span><span class="sxs-lookup"><span data-stu-id="ea971-116">String</span></span>|<span data-ttu-id="ea971-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="ea971-117">Description.</span></span> <span data-ttu-id="ea971-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ea971-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ea971-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ea971-119">omaUri</span></span>|<span data-ttu-id="ea971-120">String</span><span class="sxs-lookup"><span data-stu-id="ea971-120">String</span></span>|<span data-ttu-id="ea971-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ea971-121">OMA.</span></span> <span data-ttu-id="ea971-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ea971-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ea971-123">value</span><span class="sxs-lookup"><span data-stu-id="ea971-123">value</span></span>|<span data-ttu-id="ea971-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea971-124">Boolean</span></span>|<span data-ttu-id="ea971-125">Значение</span><span class="sxs-lookup"><span data-stu-id="ea971-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea971-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ea971-126">Relationships</span></span>
<span data-ttu-id="ea971-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ea971-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea971-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea971-128">JSON Representation</span></span>
<span data-ttu-id="ea971-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea971-129">Here is a JSON representation of the resource.</span></span>
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



