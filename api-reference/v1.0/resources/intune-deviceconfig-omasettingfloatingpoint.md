---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
ms.openlocfilehash: 649e3b3d7716122610ac60291ef58cc25e32c4e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026119"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="56a0d-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="56a0d-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="56a0d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56a0d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56a0d-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="56a0d-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="56a0d-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="56a0d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56a0d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="56a0d-107">Properties</span></span>
|<span data-ttu-id="56a0d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="56a0d-108">Property</span></span>|<span data-ttu-id="56a0d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="56a0d-109">Type</span></span>|<span data-ttu-id="56a0d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56a0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a0d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="56a0d-111">displayName</span></span>|<span data-ttu-id="56a0d-112">String</span><span class="sxs-lookup"><span data-stu-id="56a0d-112">String</span></span>|<span data-ttu-id="56a0d-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="56a0d-113">Display Name.</span></span> <span data-ttu-id="56a0d-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="56a0d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="56a0d-115">описание</span><span class="sxs-lookup"><span data-stu-id="56a0d-115">description</span></span>|<span data-ttu-id="56a0d-116">String</span><span class="sxs-lookup"><span data-stu-id="56a0d-116">String</span></span>|<span data-ttu-id="56a0d-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="56a0d-117">Description.</span></span> <span data-ttu-id="56a0d-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="56a0d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="56a0d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="56a0d-119">omaUri</span></span>|<span data-ttu-id="56a0d-120">String</span><span class="sxs-lookup"><span data-stu-id="56a0d-120">String</span></span>|<span data-ttu-id="56a0d-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="56a0d-121">OMA.</span></span> <span data-ttu-id="56a0d-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="56a0d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="56a0d-123">value</span><span class="sxs-lookup"><span data-stu-id="56a0d-123">value</span></span>|<span data-ttu-id="56a0d-124">Single</span><span class="sxs-lookup"><span data-stu-id="56a0d-124">Single</span></span>|<span data-ttu-id="56a0d-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="56a0d-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56a0d-126">Связи</span><span class="sxs-lookup"><span data-stu-id="56a0d-126">Relationships</span></span>
<span data-ttu-id="56a0d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="56a0d-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56a0d-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56a0d-128">JSON Representation</span></span>
<span data-ttu-id="56a0d-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56a0d-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



