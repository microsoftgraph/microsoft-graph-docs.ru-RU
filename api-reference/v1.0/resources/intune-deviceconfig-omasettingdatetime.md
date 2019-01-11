---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: afd66ce8838abc3ade8857ec5a4bda74144d6792
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865186"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="99cca-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="99cca-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="99cca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="99cca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99cca-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="99cca-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="99cca-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99cca-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99cca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="99cca-107">Properties</span></span>
|<span data-ttu-id="99cca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="99cca-108">Property</span></span>|<span data-ttu-id="99cca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="99cca-109">Type</span></span>|<span data-ttu-id="99cca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="99cca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99cca-111">displayName</span><span class="sxs-lookup"><span data-stu-id="99cca-111">displayName</span></span>|<span data-ttu-id="99cca-112">Строка</span><span class="sxs-lookup"><span data-stu-id="99cca-112">String</span></span>|<span data-ttu-id="99cca-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="99cca-113">Display Name.</span></span> <span data-ttu-id="99cca-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99cca-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99cca-115">описание</span><span class="sxs-lookup"><span data-stu-id="99cca-115">description</span></span>|<span data-ttu-id="99cca-116">Строка</span><span class="sxs-lookup"><span data-stu-id="99cca-116">String</span></span>|<span data-ttu-id="99cca-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="99cca-117">Description.</span></span> <span data-ttu-id="99cca-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99cca-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99cca-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="99cca-119">omaUri</span></span>|<span data-ttu-id="99cca-120">Строка</span><span class="sxs-lookup"><span data-stu-id="99cca-120">String</span></span>|<span data-ttu-id="99cca-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="99cca-121">OMA.</span></span> <span data-ttu-id="99cca-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="99cca-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="99cca-123">value</span><span class="sxs-lookup"><span data-stu-id="99cca-123">value</span></span>|<span data-ttu-id="99cca-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99cca-124">DateTimeOffset</span></span>|<span data-ttu-id="99cca-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="99cca-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99cca-126">Связи</span><span class="sxs-lookup"><span data-stu-id="99cca-126">Relationships</span></span>
<span data-ttu-id="99cca-127">Нет</span><span class="sxs-lookup"><span data-stu-id="99cca-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99cca-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99cca-128">JSON Representation</span></span>
<span data-ttu-id="99cca-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99cca-129">Here is a JSON representation of the resource.</span></span>
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



