---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
ms.openlocfilehash: 9a525d031c9f24cf18495d83e22467e103bca6d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363692"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="fc328-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="fc328-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="fc328-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc328-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc328-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="fc328-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="fc328-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc328-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc328-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc328-107">Properties</span></span>
|<span data-ttu-id="fc328-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc328-108">Property</span></span>|<span data-ttu-id="fc328-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc328-109">Type</span></span>|<span data-ttu-id="fc328-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc328-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc328-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fc328-111">displayName</span></span>|<span data-ttu-id="fc328-112">Строка</span><span class="sxs-lookup"><span data-stu-id="fc328-112">String</span></span>|<span data-ttu-id="fc328-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fc328-113">Display Name.</span></span> <span data-ttu-id="fc328-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc328-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc328-115">описание</span><span class="sxs-lookup"><span data-stu-id="fc328-115">description</span></span>|<span data-ttu-id="fc328-116">Строка</span><span class="sxs-lookup"><span data-stu-id="fc328-116">String</span></span>|<span data-ttu-id="fc328-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="fc328-117">Description.</span></span> <span data-ttu-id="fc328-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc328-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc328-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="fc328-119">omaUri</span></span>|<span data-ttu-id="fc328-120">Строка</span><span class="sxs-lookup"><span data-stu-id="fc328-120">String</span></span>|<span data-ttu-id="fc328-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="fc328-121">OMA.</span></span> <span data-ttu-id="fc328-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fc328-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fc328-123">value</span><span class="sxs-lookup"><span data-stu-id="fc328-123">value</span></span>|<span data-ttu-id="fc328-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc328-124">DateTimeOffset</span></span>|<span data-ttu-id="fc328-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="fc328-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc328-126">Связи</span><span class="sxs-lookup"><span data-stu-id="fc328-126">Relationships</span></span>
<span data-ttu-id="fc328-127">Нет</span><span class="sxs-lookup"><span data-stu-id="fc328-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc328-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc328-128">JSON Representation</span></span>
<span data-ttu-id="fc328-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc328-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



