---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34c19caee6bab30dbfe0e82abf1a55f20bb5d3b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932296"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="359ca-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="359ca-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="359ca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="359ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="359ca-105">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="359ca-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="359ca-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="359ca-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="359ca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="359ca-107">Properties</span></span>
|<span data-ttu-id="359ca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="359ca-108">Property</span></span>|<span data-ttu-id="359ca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="359ca-109">Type</span></span>|<span data-ttu-id="359ca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="359ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="359ca-111">displayName</span><span class="sxs-lookup"><span data-stu-id="359ca-111">displayName</span></span>|<span data-ttu-id="359ca-112">Строка</span><span class="sxs-lookup"><span data-stu-id="359ca-112">String</span></span>|<span data-ttu-id="359ca-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="359ca-113">Display Name.</span></span> <span data-ttu-id="359ca-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="359ca-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="359ca-115">описание</span><span class="sxs-lookup"><span data-stu-id="359ca-115">description</span></span>|<span data-ttu-id="359ca-116">Строка</span><span class="sxs-lookup"><span data-stu-id="359ca-116">String</span></span>|<span data-ttu-id="359ca-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="359ca-117">Description.</span></span> <span data-ttu-id="359ca-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="359ca-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="359ca-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="359ca-119">omaUri</span></span>|<span data-ttu-id="359ca-120">Строка</span><span class="sxs-lookup"><span data-stu-id="359ca-120">String</span></span>|<span data-ttu-id="359ca-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="359ca-121">OMA.</span></span> <span data-ttu-id="359ca-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="359ca-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="359ca-123">value</span><span class="sxs-lookup"><span data-stu-id="359ca-123">value</span></span>|<span data-ttu-id="359ca-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359ca-124">DateTimeOffset</span></span>|<span data-ttu-id="359ca-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="359ca-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="359ca-126">Связи</span><span class="sxs-lookup"><span data-stu-id="359ca-126">Relationships</span></span>
<span data-ttu-id="359ca-127">Нет</span><span class="sxs-lookup"><span data-stu-id="359ca-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="359ca-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="359ca-128">JSON Representation</span></span>
<span data-ttu-id="359ca-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="359ca-129">Here is a JSON representation of the resource.</span></span>
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



