---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
ms.openlocfilehash: 1c0cc1d90374b7720fd9ba95e7488a09167f7842
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025787"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="ac2a4-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="ac2a4-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="ac2a4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac2a4-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="ac2a4-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac2a4-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac2a4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac2a4-107">Properties</span></span>
|<span data-ttu-id="ac2a4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac2a4-108">Property</span></span>|<span data-ttu-id="ac2a4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac2a4-109">Type</span></span>|<span data-ttu-id="ac2a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac2a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac2a4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ac2a4-111">displayName</span></span>|<span data-ttu-id="ac2a4-112">String</span><span class="sxs-lookup"><span data-stu-id="ac2a4-112">String</span></span>|<span data-ttu-id="ac2a4-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-113">Display Name.</span></span> <span data-ttu-id="ac2a4-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac2a4-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac2a4-115">описание</span><span class="sxs-lookup"><span data-stu-id="ac2a4-115">description</span></span>|<span data-ttu-id="ac2a4-116">String</span><span class="sxs-lookup"><span data-stu-id="ac2a4-116">String</span></span>|<span data-ttu-id="ac2a4-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-117">Description.</span></span> <span data-ttu-id="ac2a4-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac2a4-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac2a4-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ac2a4-119">omaUri</span></span>|<span data-ttu-id="ac2a4-120">String</span><span class="sxs-lookup"><span data-stu-id="ac2a4-120">String</span></span>|<span data-ttu-id="ac2a4-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-121">OMA.</span></span> <span data-ttu-id="ac2a4-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac2a4-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac2a4-123">value</span><span class="sxs-lookup"><span data-stu-id="ac2a4-123">value</span></span>|<span data-ttu-id="ac2a4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac2a4-124">Boolean</span></span>|<span data-ttu-id="ac2a4-125">Значение</span><span class="sxs-lookup"><span data-stu-id="ac2a4-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac2a4-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ac2a4-126">Relationships</span></span>
<span data-ttu-id="ac2a4-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ac2a4-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac2a4-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac2a4-128">JSON Representation</span></span>
<span data-ttu-id="ac2a4-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac2a4-129">Here is a JSON representation of the resource.</span></span>
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



