---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
ms.openlocfilehash: efed2112f85ee0600fcbe499616a7f3e787beb59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360755"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="ac50a-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="ac50a-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="ac50a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac50a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac50a-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="ac50a-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="ac50a-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac50a-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac50a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac50a-107">Properties</span></span>
|<span data-ttu-id="ac50a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac50a-108">Property</span></span>|<span data-ttu-id="ac50a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac50a-109">Type</span></span>|<span data-ttu-id="ac50a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac50a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac50a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ac50a-111">displayName</span></span>|<span data-ttu-id="ac50a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ac50a-112">String</span></span>|<span data-ttu-id="ac50a-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ac50a-113">Display Name.</span></span> <span data-ttu-id="ac50a-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac50a-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac50a-115">описание</span><span class="sxs-lookup"><span data-stu-id="ac50a-115">description</span></span>|<span data-ttu-id="ac50a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ac50a-116">String</span></span>|<span data-ttu-id="ac50a-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="ac50a-117">Description.</span></span> <span data-ttu-id="ac50a-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac50a-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac50a-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ac50a-119">omaUri</span></span>|<span data-ttu-id="ac50a-120">Строка</span><span class="sxs-lookup"><span data-stu-id="ac50a-120">String</span></span>|<span data-ttu-id="ac50a-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="ac50a-121">OMA.</span></span> <span data-ttu-id="ac50a-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ac50a-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ac50a-123">value</span><span class="sxs-lookup"><span data-stu-id="ac50a-123">value</span></span>|<span data-ttu-id="ac50a-124">Single</span><span class="sxs-lookup"><span data-stu-id="ac50a-124">Single</span></span>|<span data-ttu-id="ac50a-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="ac50a-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac50a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ac50a-126">Relationships</span></span>
<span data-ttu-id="ac50a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ac50a-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac50a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac50a-128">JSON Representation</span></span>
<span data-ttu-id="ac50a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac50a-129">Here is a JSON representation of the resource.</span></span>
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



