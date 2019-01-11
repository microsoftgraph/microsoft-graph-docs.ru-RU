---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b62d012b39aa258bd3754f57109eb265c397ccb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850129"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="74198-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="74198-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="74198-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74198-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74198-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74198-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74198-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74198-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74198-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="74198-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="74198-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74198-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74198-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="74198-109">Properties</span></span>
|<span data-ttu-id="74198-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="74198-110">Property</span></span>|<span data-ttu-id="74198-111">Тип</span><span class="sxs-lookup"><span data-stu-id="74198-111">Type</span></span>|<span data-ttu-id="74198-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74198-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74198-113">displayName</span><span class="sxs-lookup"><span data-stu-id="74198-113">displayName</span></span>|<span data-ttu-id="74198-114">Строка</span><span class="sxs-lookup"><span data-stu-id="74198-114">String</span></span>|<span data-ttu-id="74198-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="74198-115">Display Name.</span></span> <span data-ttu-id="74198-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74198-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74198-117">описание</span><span class="sxs-lookup"><span data-stu-id="74198-117">description</span></span>|<span data-ttu-id="74198-118">Строка</span><span class="sxs-lookup"><span data-stu-id="74198-118">String</span></span>|<span data-ttu-id="74198-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="74198-119">Description.</span></span> <span data-ttu-id="74198-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74198-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74198-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="74198-121">omaUri</span></span>|<span data-ttu-id="74198-122">Строка</span><span class="sxs-lookup"><span data-stu-id="74198-122">String</span></span>|<span data-ttu-id="74198-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="74198-123">OMA.</span></span> <span data-ttu-id="74198-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="74198-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="74198-125">value</span><span class="sxs-lookup"><span data-stu-id="74198-125">value</span></span>|<span data-ttu-id="74198-126">Int32</span><span class="sxs-lookup"><span data-stu-id="74198-126">Int32</span></span>|<span data-ttu-id="74198-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="74198-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74198-128">Связи</span><span class="sxs-lookup"><span data-stu-id="74198-128">Relationships</span></span>
<span data-ttu-id="74198-129">Нет</span><span class="sxs-lookup"><span data-stu-id="74198-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74198-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74198-130">JSON Representation</span></span>
<span data-ttu-id="74198-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74198-131">Here is a JSON representation of the resource.</span></span>
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





