---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46bca1f6052dae3f4699b88258abce4b346c67bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868210"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="f82f6-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="f82f6-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="f82f6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f82f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f82f6-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="f82f6-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="f82f6-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f82f6-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f82f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f82f6-107">Properties</span></span>
|<span data-ttu-id="f82f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f82f6-108">Property</span></span>|<span data-ttu-id="f82f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f82f6-109">Type</span></span>|<span data-ttu-id="f82f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f82f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f82f6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f82f6-111">displayName</span></span>|<span data-ttu-id="f82f6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f82f6-112">String</span></span>|<span data-ttu-id="f82f6-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f82f6-113">Display Name.</span></span> <span data-ttu-id="f82f6-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f82f6-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f82f6-115">описание</span><span class="sxs-lookup"><span data-stu-id="f82f6-115">description</span></span>|<span data-ttu-id="f82f6-116">Строка</span><span class="sxs-lookup"><span data-stu-id="f82f6-116">String</span></span>|<span data-ttu-id="f82f6-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="f82f6-117">Description.</span></span> <span data-ttu-id="f82f6-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f82f6-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f82f6-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f82f6-119">omaUri</span></span>|<span data-ttu-id="f82f6-120">Строка</span><span class="sxs-lookup"><span data-stu-id="f82f6-120">String</span></span>|<span data-ttu-id="f82f6-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="f82f6-121">OMA.</span></span> <span data-ttu-id="f82f6-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f82f6-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f82f6-123">value</span><span class="sxs-lookup"><span data-stu-id="f82f6-123">value</span></span>|<span data-ttu-id="f82f6-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f82f6-124">Boolean</span></span>|<span data-ttu-id="f82f6-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f82f6-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f82f6-126">Связи</span><span class="sxs-lookup"><span data-stu-id="f82f6-126">Relationships</span></span>
<span data-ttu-id="f82f6-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f82f6-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f82f6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f82f6-128">JSON Representation</span></span>
<span data-ttu-id="f82f6-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f82f6-129">Here is a JSON representation of the resource.</span></span>
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



