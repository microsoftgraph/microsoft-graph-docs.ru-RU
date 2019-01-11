---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f40d5d225c2b4b99573c482b39f886bcd463e9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860454"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="2ab19-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="2ab19-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="2ab19-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ab19-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab19-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="2ab19-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="2ab19-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ab19-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ab19-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ab19-107">Properties</span></span>
|<span data-ttu-id="2ab19-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ab19-108">Property</span></span>|<span data-ttu-id="2ab19-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ab19-109">Type</span></span>|<span data-ttu-id="2ab19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab19-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ab19-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2ab19-111">displayName</span></span>|<span data-ttu-id="2ab19-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab19-112">String</span></span>|<span data-ttu-id="2ab19-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2ab19-113">Display Name.</span></span> <span data-ttu-id="2ab19-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ab19-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ab19-115">описание</span><span class="sxs-lookup"><span data-stu-id="2ab19-115">description</span></span>|<span data-ttu-id="2ab19-116">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab19-116">String</span></span>|<span data-ttu-id="2ab19-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="2ab19-117">Description.</span></span> <span data-ttu-id="2ab19-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ab19-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ab19-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="2ab19-119">omaUri</span></span>|<span data-ttu-id="2ab19-120">Строка</span><span class="sxs-lookup"><span data-stu-id="2ab19-120">String</span></span>|<span data-ttu-id="2ab19-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="2ab19-121">OMA.</span></span> <span data-ttu-id="2ab19-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ab19-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ab19-123">value</span><span class="sxs-lookup"><span data-stu-id="2ab19-123">value</span></span>|<span data-ttu-id="2ab19-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2ab19-124">Int32</span></span>|<span data-ttu-id="2ab19-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="2ab19-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ab19-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2ab19-126">Relationships</span></span>
<span data-ttu-id="2ab19-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2ab19-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ab19-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ab19-128">JSON Representation</span></span>
<span data-ttu-id="2ab19-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ab19-129">Here is a JSON representation of the resource.</span></span>
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



