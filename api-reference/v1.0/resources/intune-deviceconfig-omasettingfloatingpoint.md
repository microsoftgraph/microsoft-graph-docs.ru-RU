---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a36d30cb62862b469d7b32d742275d399ed36db0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888132"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="2e700-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="2e700-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="2e700-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e700-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e700-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="2e700-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="2e700-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2e700-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e700-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e700-107">Properties</span></span>
|<span data-ttu-id="2e700-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e700-108">Property</span></span>|<span data-ttu-id="2e700-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e700-109">Type</span></span>|<span data-ttu-id="2e700-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e700-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e700-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2e700-111">displayName</span></span>|<span data-ttu-id="2e700-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2e700-112">String</span></span>|<span data-ttu-id="2e700-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2e700-113">Display Name.</span></span> <span data-ttu-id="2e700-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2e700-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2e700-115">описание</span><span class="sxs-lookup"><span data-stu-id="2e700-115">description</span></span>|<span data-ttu-id="2e700-116">Строка</span><span class="sxs-lookup"><span data-stu-id="2e700-116">String</span></span>|<span data-ttu-id="2e700-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="2e700-117">Description.</span></span> <span data-ttu-id="2e700-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2e700-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2e700-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="2e700-119">omaUri</span></span>|<span data-ttu-id="2e700-120">Строка</span><span class="sxs-lookup"><span data-stu-id="2e700-120">String</span></span>|<span data-ttu-id="2e700-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="2e700-121">OMA.</span></span> <span data-ttu-id="2e700-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2e700-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2e700-123">value</span><span class="sxs-lookup"><span data-stu-id="2e700-123">value</span></span>|<span data-ttu-id="2e700-124">Single</span><span class="sxs-lookup"><span data-stu-id="2e700-124">Single</span></span>|<span data-ttu-id="2e700-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="2e700-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e700-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2e700-126">Relationships</span></span>
<span data-ttu-id="2e700-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2e700-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e700-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e700-128">JSON Representation</span></span>
<span data-ttu-id="2e700-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e700-129">Here is a JSON representation of the resource.</span></span>
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



