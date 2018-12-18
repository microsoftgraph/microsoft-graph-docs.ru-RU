---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
ms.openlocfilehash: 6a2e6fe6e6782159afa99d91785ae9e854a2e99c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306554"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="8949d-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="8949d-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="8949d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8949d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8949d-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="8949d-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="8949d-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8949d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8949d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8949d-107">Properties</span></span>
|<span data-ttu-id="8949d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8949d-108">Property</span></span>|<span data-ttu-id="8949d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8949d-109">Type</span></span>|<span data-ttu-id="8949d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8949d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8949d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8949d-111">displayName</span></span>|<span data-ttu-id="8949d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8949d-112">String</span></span>|<span data-ttu-id="8949d-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="8949d-113">Display Name.</span></span> <span data-ttu-id="8949d-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8949d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8949d-115">описание</span><span class="sxs-lookup"><span data-stu-id="8949d-115">description</span></span>|<span data-ttu-id="8949d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8949d-116">String</span></span>|<span data-ttu-id="8949d-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="8949d-117">Description.</span></span> <span data-ttu-id="8949d-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8949d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8949d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8949d-119">omaUri</span></span>|<span data-ttu-id="8949d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="8949d-120">String</span></span>|<span data-ttu-id="8949d-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8949d-121">OMA.</span></span> <span data-ttu-id="8949d-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8949d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8949d-123">value</span><span class="sxs-lookup"><span data-stu-id="8949d-123">value</span></span>|<span data-ttu-id="8949d-124">Int32</span><span class="sxs-lookup"><span data-stu-id="8949d-124">Int32</span></span>|<span data-ttu-id="8949d-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="8949d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8949d-126">Связи</span><span class="sxs-lookup"><span data-stu-id="8949d-126">Relationships</span></span>
<span data-ttu-id="8949d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="8949d-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8949d-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8949d-128">JSON Representation</span></span>
<span data-ttu-id="8949d-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8949d-129">Here is a JSON representation of the resource.</span></span>
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



