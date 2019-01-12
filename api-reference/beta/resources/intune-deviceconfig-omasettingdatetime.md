---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4552eef8ec9237c45b1e2b98404977a48e99a896
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942544"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="c2b20-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="c2b20-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="c2b20-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2b20-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2b20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2b20-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2b20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2b20-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c2b20-107">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="c2b20-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2b20-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2b20-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2b20-109">Properties</span></span>
|<span data-ttu-id="c2b20-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2b20-110">Property</span></span>|<span data-ttu-id="c2b20-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b20-111">Type</span></span>|<span data-ttu-id="c2b20-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b20-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b20-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c2b20-113">displayName</span></span>|<span data-ttu-id="c2b20-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c2b20-114">String</span></span>|<span data-ttu-id="c2b20-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2b20-115">Display Name.</span></span> <span data-ttu-id="c2b20-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2b20-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2b20-117">описание</span><span class="sxs-lookup"><span data-stu-id="c2b20-117">description</span></span>|<span data-ttu-id="c2b20-118">Строка</span><span class="sxs-lookup"><span data-stu-id="c2b20-118">String</span></span>|<span data-ttu-id="c2b20-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="c2b20-119">Description.</span></span> <span data-ttu-id="c2b20-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2b20-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2b20-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="c2b20-121">omaUri</span></span>|<span data-ttu-id="c2b20-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c2b20-122">String</span></span>|<span data-ttu-id="c2b20-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="c2b20-123">OMA.</span></span> <span data-ttu-id="c2b20-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2b20-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2b20-125">value</span><span class="sxs-lookup"><span data-stu-id="c2b20-125">value</span></span>|<span data-ttu-id="c2b20-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2b20-126">DateTimeOffset</span></span>|<span data-ttu-id="c2b20-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="c2b20-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2b20-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c2b20-128">Relationships</span></span>
<span data-ttu-id="c2b20-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c2b20-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2b20-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2b20-130">JSON Representation</span></span>
<span data-ttu-id="c2b20-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2b20-131">Here is a JSON representation of the resource.</span></span>
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





