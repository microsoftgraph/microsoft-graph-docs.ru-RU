---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
ms.openlocfilehash: 10101217d1c0f07931cb847e1c14f36844c8dc9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323284"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="e2ee0-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="e2ee0-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="e2ee0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2ee0-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="e2ee0-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2ee0-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2ee0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2ee0-107">Properties</span></span>
|<span data-ttu-id="e2ee0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2ee0-108">Property</span></span>|<span data-ttu-id="e2ee0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ee0-109">Type</span></span>|<span data-ttu-id="e2ee0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ee0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ee0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e2ee0-111">displayName</span></span>|<span data-ttu-id="e2ee0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e2ee0-112">String</span></span>|<span data-ttu-id="e2ee0-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-113">Display Name.</span></span> <span data-ttu-id="e2ee0-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2ee0-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2ee0-115">описание</span><span class="sxs-lookup"><span data-stu-id="e2ee0-115">description</span></span>|<span data-ttu-id="e2ee0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="e2ee0-116">String</span></span>|<span data-ttu-id="e2ee0-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-117">Description.</span></span> <span data-ttu-id="e2ee0-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2ee0-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2ee0-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e2ee0-119">omaUri</span></span>|<span data-ttu-id="e2ee0-120">Строка</span><span class="sxs-lookup"><span data-stu-id="e2ee0-120">String</span></span>|<span data-ttu-id="e2ee0-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-121">OMA.</span></span> <span data-ttu-id="e2ee0-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2ee0-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e2ee0-123">value</span><span class="sxs-lookup"><span data-stu-id="e2ee0-123">value</span></span>|<span data-ttu-id="e2ee0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2ee0-124">Boolean</span></span>|<span data-ttu-id="e2ee0-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e2ee0-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ee0-126">Связи</span><span class="sxs-lookup"><span data-stu-id="e2ee0-126">Relationships</span></span>
<span data-ttu-id="e2ee0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="e2ee0-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2ee0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2ee0-128">JSON Representation</span></span>
<span data-ttu-id="e2ee0-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2ee0-129">Here is a JSON representation of the resource.</span></span>
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



