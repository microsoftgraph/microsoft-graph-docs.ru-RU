---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
ms.openlocfilehash: c81e4aa257bf2ddf61bbb27613a44dab92af5a82
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082702"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="9e976-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="9e976-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="9e976-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e976-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e976-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e976-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e976-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9e976-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e976-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="9e976-107">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="9e976-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e976-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e976-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e976-109">Properties</span></span>
|<span data-ttu-id="9e976-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e976-110">Property</span></span>|<span data-ttu-id="9e976-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9e976-111">Type</span></span>|<span data-ttu-id="9e976-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9e976-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e976-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9e976-113">displayName</span></span>|<span data-ttu-id="9e976-114">String</span><span class="sxs-lookup"><span data-stu-id="9e976-114">String</span></span>|<span data-ttu-id="9e976-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9e976-115">Display Name.</span></span> <span data-ttu-id="9e976-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e976-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9e976-117">описание</span><span class="sxs-lookup"><span data-stu-id="9e976-117">description</span></span>|<span data-ttu-id="9e976-118">String</span><span class="sxs-lookup"><span data-stu-id="9e976-118">String</span></span>|<span data-ttu-id="9e976-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="9e976-119">Description.</span></span> <span data-ttu-id="9e976-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e976-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9e976-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9e976-121">omaUri</span></span>|<span data-ttu-id="9e976-122">String</span><span class="sxs-lookup"><span data-stu-id="9e976-122">String</span></span>|<span data-ttu-id="9e976-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="9e976-123">OMA.</span></span> <span data-ttu-id="9e976-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9e976-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9e976-125">value</span><span class="sxs-lookup"><span data-stu-id="9e976-125">value</span></span>|<span data-ttu-id="9e976-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e976-126">DateTimeOffset</span></span>|<span data-ttu-id="9e976-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="9e976-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e976-128">Связи</span><span class="sxs-lookup"><span data-stu-id="9e976-128">Relationships</span></span>
<span data-ttu-id="9e976-129">Нет</span><span class="sxs-lookup"><span data-stu-id="9e976-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e976-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e976-130">JSON Representation</span></span>
<span data-ttu-id="9e976-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e976-131">Here is a JSON representation of the resource.</span></span>
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





