---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
ms.openlocfilehash: 2bf55308c230ec848f7ee58f66e710f1b31c1692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307989"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="bf6fc-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="bf6fc-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="bf6fc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf6fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf6fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf6fc-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-107">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="bf6fc-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bf6fc-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf6fc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf6fc-109">Properties</span></span>
|<span data-ttu-id="bf6fc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf6fc-110">Property</span></span>|<span data-ttu-id="bf6fc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bf6fc-111">Type</span></span>|<span data-ttu-id="bf6fc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6fc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6fc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bf6fc-113">displayName</span></span>|<span data-ttu-id="bf6fc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="bf6fc-114">String</span></span>|<span data-ttu-id="bf6fc-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-115">Display Name.</span></span> <span data-ttu-id="bf6fc-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bf6fc-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf6fc-117">описание</span><span class="sxs-lookup"><span data-stu-id="bf6fc-117">description</span></span>|<span data-ttu-id="bf6fc-118">Строка</span><span class="sxs-lookup"><span data-stu-id="bf6fc-118">String</span></span>|<span data-ttu-id="bf6fc-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-119">Description.</span></span> <span data-ttu-id="bf6fc-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bf6fc-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf6fc-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="bf6fc-121">omaUri</span></span>|<span data-ttu-id="bf6fc-122">Строка</span><span class="sxs-lookup"><span data-stu-id="bf6fc-122">String</span></span>|<span data-ttu-id="bf6fc-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-123">OMA.</span></span> <span data-ttu-id="bf6fc-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bf6fc-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf6fc-125">value</span><span class="sxs-lookup"><span data-stu-id="bf6fc-125">value</span></span>|<span data-ttu-id="bf6fc-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf6fc-126">DateTimeOffset</span></span>|<span data-ttu-id="bf6fc-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf6fc-128">Связи</span><span class="sxs-lookup"><span data-stu-id="bf6fc-128">Relationships</span></span>
<span data-ttu-id="bf6fc-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bf6fc-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf6fc-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf6fc-130">JSON Representation</span></span>
<span data-ttu-id="bf6fc-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf6fc-131">Here is a JSON representation of the resource.</span></span>
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





