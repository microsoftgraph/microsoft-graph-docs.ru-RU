---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46398e43f2a7ea224a07b1637deca2c3a6ed067
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987533"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="08c5a-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="08c5a-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="08c5a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08c5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08c5a-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="08c5a-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="08c5a-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08c5a-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08c5a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08c5a-107">Properties</span></span>
|<span data-ttu-id="08c5a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08c5a-108">Property</span></span>|<span data-ttu-id="08c5a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08c5a-109">Type</span></span>|<span data-ttu-id="08c5a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08c5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c5a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="08c5a-111">displayName</span></span>|<span data-ttu-id="08c5a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="08c5a-112">String</span></span>|<span data-ttu-id="08c5a-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="08c5a-113">Display Name.</span></span> <span data-ttu-id="08c5a-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08c5a-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08c5a-115">описание</span><span class="sxs-lookup"><span data-stu-id="08c5a-115">description</span></span>|<span data-ttu-id="08c5a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="08c5a-116">String</span></span>|<span data-ttu-id="08c5a-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="08c5a-117">Description.</span></span> <span data-ttu-id="08c5a-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08c5a-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08c5a-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="08c5a-119">omaUri</span></span>|<span data-ttu-id="08c5a-120">Строка</span><span class="sxs-lookup"><span data-stu-id="08c5a-120">String</span></span>|<span data-ttu-id="08c5a-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="08c5a-121">OMA.</span></span> <span data-ttu-id="08c5a-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="08c5a-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="08c5a-123">value</span><span class="sxs-lookup"><span data-stu-id="08c5a-123">value</span></span>|<span data-ttu-id="08c5a-124">Int32</span><span class="sxs-lookup"><span data-stu-id="08c5a-124">Int32</span></span>|<span data-ttu-id="08c5a-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="08c5a-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08c5a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="08c5a-126">Relationships</span></span>
<span data-ttu-id="08c5a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="08c5a-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08c5a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08c5a-128">JSON Representation</span></span>
<span data-ttu-id="08c5a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08c5a-129">Here is a JSON representation of the resource.</span></span>
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



