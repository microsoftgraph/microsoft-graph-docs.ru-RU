---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
ms.openlocfilehash: b4ea11c22acb2a4119c2de1934f1ae66c2310658
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025112"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="07771-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="07771-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="07771-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07771-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07771-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="07771-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="07771-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07771-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07771-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="07771-107">Properties</span></span>
|<span data-ttu-id="07771-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="07771-108">Property</span></span>|<span data-ttu-id="07771-109">Тип</span><span class="sxs-lookup"><span data-stu-id="07771-109">Type</span></span>|<span data-ttu-id="07771-110">Описание</span><span class="sxs-lookup"><span data-stu-id="07771-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07771-111">displayName</span><span class="sxs-lookup"><span data-stu-id="07771-111">displayName</span></span>|<span data-ttu-id="07771-112">String</span><span class="sxs-lookup"><span data-stu-id="07771-112">String</span></span>|<span data-ttu-id="07771-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="07771-113">Display Name.</span></span> <span data-ttu-id="07771-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07771-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07771-115">описание</span><span class="sxs-lookup"><span data-stu-id="07771-115">description</span></span>|<span data-ttu-id="07771-116">String</span><span class="sxs-lookup"><span data-stu-id="07771-116">String</span></span>|<span data-ttu-id="07771-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="07771-117">Description.</span></span> <span data-ttu-id="07771-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07771-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07771-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="07771-119">omaUri</span></span>|<span data-ttu-id="07771-120">String</span><span class="sxs-lookup"><span data-stu-id="07771-120">String</span></span>|<span data-ttu-id="07771-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="07771-121">OMA.</span></span> <span data-ttu-id="07771-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07771-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07771-123">value</span><span class="sxs-lookup"><span data-stu-id="07771-123">value</span></span>|<span data-ttu-id="07771-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07771-124">DateTimeOffset</span></span>|<span data-ttu-id="07771-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="07771-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07771-126">Связи</span><span class="sxs-lookup"><span data-stu-id="07771-126">Relationships</span></span>
<span data-ttu-id="07771-127">Нет</span><span class="sxs-lookup"><span data-stu-id="07771-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07771-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07771-128">JSON Representation</span></span>
<span data-ttu-id="07771-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07771-129">Here is a JSON representation of the resource.</span></span>
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



