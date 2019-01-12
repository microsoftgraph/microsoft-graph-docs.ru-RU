---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0b3f2d04c9476cc10a67c1e68ba9a29288e8875
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986637"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="a9891-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="a9891-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="a9891-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9891-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9891-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="a9891-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="a9891-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9891-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9891-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9891-107">Properties</span></span>
|<span data-ttu-id="a9891-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9891-108">Property</span></span>|<span data-ttu-id="a9891-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a9891-109">Type</span></span>|<span data-ttu-id="a9891-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a9891-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9891-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a9891-111">displayName</span></span>|<span data-ttu-id="a9891-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a9891-112">String</span></span>|<span data-ttu-id="a9891-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a9891-113">Display Name.</span></span> <span data-ttu-id="a9891-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9891-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9891-115">описание</span><span class="sxs-lookup"><span data-stu-id="a9891-115">description</span></span>|<span data-ttu-id="a9891-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a9891-116">String</span></span>|<span data-ttu-id="a9891-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="a9891-117">Description.</span></span> <span data-ttu-id="a9891-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9891-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9891-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="a9891-119">omaUri</span></span>|<span data-ttu-id="a9891-120">Строка</span><span class="sxs-lookup"><span data-stu-id="a9891-120">String</span></span>|<span data-ttu-id="a9891-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="a9891-121">OMA.</span></span> <span data-ttu-id="a9891-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a9891-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a9891-123">value</span><span class="sxs-lookup"><span data-stu-id="a9891-123">value</span></span>|<span data-ttu-id="a9891-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9891-124">Boolean</span></span>|<span data-ttu-id="a9891-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a9891-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9891-126">Связи</span><span class="sxs-lookup"><span data-stu-id="a9891-126">Relationships</span></span>
<span data-ttu-id="a9891-127">Нет</span><span class="sxs-lookup"><span data-stu-id="a9891-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9891-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9891-128">JSON Representation</span></span>
<span data-ttu-id="a9891-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9891-129">Here is a JSON representation of the resource.</span></span>
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



