---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 890d636afb29fbfb188e9c1b514eecc6360001b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841351"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="f0dd0-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="f0dd0-103">omaSettingString resource type</span></span>

> <span data-ttu-id="f0dd0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0dd0-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-105">OMA Settings String definition.</span></span>

<span data-ttu-id="f0dd0-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0dd0-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0dd0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0dd0-107">Properties</span></span>
|<span data-ttu-id="f0dd0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0dd0-108">Property</span></span>|<span data-ttu-id="f0dd0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0dd0-109">Type</span></span>|<span data-ttu-id="f0dd0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0dd0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0dd0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f0dd0-111">displayName</span></span>|<span data-ttu-id="f0dd0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f0dd0-112">String</span></span>|<span data-ttu-id="f0dd0-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-113">Display Name.</span></span> <span data-ttu-id="f0dd0-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0dd0-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0dd0-115">описание</span><span class="sxs-lookup"><span data-stu-id="f0dd0-115">description</span></span>|<span data-ttu-id="f0dd0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="f0dd0-116">String</span></span>|<span data-ttu-id="f0dd0-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-117">Description.</span></span> <span data-ttu-id="f0dd0-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0dd0-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0dd0-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f0dd0-119">omaUri</span></span>|<span data-ttu-id="f0dd0-120">Строка</span><span class="sxs-lookup"><span data-stu-id="f0dd0-120">String</span></span>|<span data-ttu-id="f0dd0-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-121">OMA.</span></span> <span data-ttu-id="f0dd0-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f0dd0-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f0dd0-123">value</span><span class="sxs-lookup"><span data-stu-id="f0dd0-123">value</span></span>|<span data-ttu-id="f0dd0-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f0dd0-124">String</span></span>|<span data-ttu-id="f0dd0-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f0dd0-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0dd0-126">Связи</span><span class="sxs-lookup"><span data-stu-id="f0dd0-126">Relationships</span></span>
<span data-ttu-id="f0dd0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f0dd0-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0dd0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0dd0-128">JSON Representation</span></span>
<span data-ttu-id="f0dd0-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0dd0-129">Here is a JSON representation of the resource.</span></span>
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



