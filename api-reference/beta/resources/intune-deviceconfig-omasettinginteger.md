---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
ms.openlocfilehash: 27d38d1e1fe035ef95203ca1e636dedf7a05f103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363608"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="06570-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="06570-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="06570-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06570-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06570-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06570-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06570-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06570-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06570-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="06570-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="06570-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06570-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06570-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="06570-109">Properties</span></span>
|<span data-ttu-id="06570-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="06570-110">Property</span></span>|<span data-ttu-id="06570-111">Тип</span><span class="sxs-lookup"><span data-stu-id="06570-111">Type</span></span>|<span data-ttu-id="06570-112">Описание</span><span class="sxs-lookup"><span data-stu-id="06570-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06570-113">displayName</span><span class="sxs-lookup"><span data-stu-id="06570-113">displayName</span></span>|<span data-ttu-id="06570-114">Строка</span><span class="sxs-lookup"><span data-stu-id="06570-114">String</span></span>|<span data-ttu-id="06570-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="06570-115">Display Name.</span></span> <span data-ttu-id="06570-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06570-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06570-117">описание</span><span class="sxs-lookup"><span data-stu-id="06570-117">description</span></span>|<span data-ttu-id="06570-118">Строка</span><span class="sxs-lookup"><span data-stu-id="06570-118">String</span></span>|<span data-ttu-id="06570-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="06570-119">Description.</span></span> <span data-ttu-id="06570-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06570-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06570-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="06570-121">omaUri</span></span>|<span data-ttu-id="06570-122">Строка</span><span class="sxs-lookup"><span data-stu-id="06570-122">String</span></span>|<span data-ttu-id="06570-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="06570-123">OMA.</span></span> <span data-ttu-id="06570-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="06570-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="06570-125">value</span><span class="sxs-lookup"><span data-stu-id="06570-125">value</span></span>|<span data-ttu-id="06570-126">Int32</span><span class="sxs-lookup"><span data-stu-id="06570-126">Int32</span></span>|<span data-ttu-id="06570-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="06570-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06570-128">Связи</span><span class="sxs-lookup"><span data-stu-id="06570-128">Relationships</span></span>
<span data-ttu-id="06570-129">Нет</span><span class="sxs-lookup"><span data-stu-id="06570-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06570-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06570-130">JSON Representation</span></span>
<span data-ttu-id="06570-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06570-131">Here is a JSON representation of the resource.</span></span>
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





