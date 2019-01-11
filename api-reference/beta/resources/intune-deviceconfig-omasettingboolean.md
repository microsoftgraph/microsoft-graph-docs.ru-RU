---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a213f75345fbd3b17a103124ae192e62b79a1007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875861"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="07fe3-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="07fe3-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="07fe3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07fe3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07fe3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07fe3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07fe3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07fe3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07fe3-107">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="07fe3-107">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="07fe3-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07fe3-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07fe3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="07fe3-109">Properties</span></span>
|<span data-ttu-id="07fe3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="07fe3-110">Property</span></span>|<span data-ttu-id="07fe3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="07fe3-111">Type</span></span>|<span data-ttu-id="07fe3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="07fe3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07fe3-113">displayName</span><span class="sxs-lookup"><span data-stu-id="07fe3-113">displayName</span></span>|<span data-ttu-id="07fe3-114">Строка</span><span class="sxs-lookup"><span data-stu-id="07fe3-114">String</span></span>|<span data-ttu-id="07fe3-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="07fe3-115">Display Name.</span></span> <span data-ttu-id="07fe3-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07fe3-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07fe3-117">описание</span><span class="sxs-lookup"><span data-stu-id="07fe3-117">description</span></span>|<span data-ttu-id="07fe3-118">Строка</span><span class="sxs-lookup"><span data-stu-id="07fe3-118">String</span></span>|<span data-ttu-id="07fe3-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="07fe3-119">Description.</span></span> <span data-ttu-id="07fe3-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07fe3-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07fe3-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="07fe3-121">omaUri</span></span>|<span data-ttu-id="07fe3-122">Строка</span><span class="sxs-lookup"><span data-stu-id="07fe3-122">String</span></span>|<span data-ttu-id="07fe3-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="07fe3-123">OMA.</span></span> <span data-ttu-id="07fe3-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="07fe3-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="07fe3-125">value</span><span class="sxs-lookup"><span data-stu-id="07fe3-125">value</span></span>|<span data-ttu-id="07fe3-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="07fe3-126">Boolean</span></span>|<span data-ttu-id="07fe3-127">Значение</span><span class="sxs-lookup"><span data-stu-id="07fe3-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07fe3-128">Связи</span><span class="sxs-lookup"><span data-stu-id="07fe3-128">Relationships</span></span>
<span data-ttu-id="07fe3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="07fe3-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07fe3-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07fe3-130">JSON Representation</span></span>
<span data-ttu-id="07fe3-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07fe3-131">Here is a JSON representation of the resource.</span></span>
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





