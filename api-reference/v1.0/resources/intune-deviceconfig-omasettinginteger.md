---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253556"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="08e85-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="08e85-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="08e85-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08e85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e85-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="08e85-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="08e85-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08e85-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08e85-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08e85-107">Properties</span></span>
|<span data-ttu-id="08e85-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08e85-108">Property</span></span>|<span data-ttu-id="08e85-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08e85-109">Type</span></span>|<span data-ttu-id="08e85-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08e85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e85-111">displayName</span><span class="sxs-lookup"><span data-stu-id="08e85-111">displayName</span></span>|<span data-ttu-id="08e85-112">String</span><span class="sxs-lookup"><span data-stu-id="08e85-112">String</span></span>|<span data-ttu-id="08e85-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="08e85-113">Display Name.</span></span> <span data-ttu-id="08e85-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08e85-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08e85-115">description</span><span class="sxs-lookup"><span data-stu-id="08e85-115">description</span></span>|<span data-ttu-id="08e85-116">String</span><span class="sxs-lookup"><span data-stu-id="08e85-116">String</span></span>|<span data-ttu-id="08e85-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="08e85-117">Description.</span></span> <span data-ttu-id="08e85-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08e85-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08e85-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="08e85-119">omaUri</span></span>|<span data-ttu-id="08e85-120">String</span><span class="sxs-lookup"><span data-stu-id="08e85-120">String</span></span>|<span data-ttu-id="08e85-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="08e85-121">OMA.</span></span> <span data-ttu-id="08e85-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08e85-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08e85-123">value</span><span class="sxs-lookup"><span data-stu-id="08e85-123">value</span></span>|<span data-ttu-id="08e85-124">Int32</span><span class="sxs-lookup"><span data-stu-id="08e85-124">Int32</span></span>|<span data-ttu-id="08e85-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="08e85-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08e85-126">Связи</span><span class="sxs-lookup"><span data-stu-id="08e85-126">Relationships</span></span>
<span data-ttu-id="08e85-127">Нет</span><span class="sxs-lookup"><span data-stu-id="08e85-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08e85-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08e85-128">JSON Representation</span></span>
<span data-ttu-id="08e85-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e85-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



