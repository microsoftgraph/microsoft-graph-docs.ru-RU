---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
ms.openlocfilehash: 543b993ee557c47e415a2f19f9791b0685c818e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025384"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="13b38-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="13b38-103">omaSettingString resource type</span></span>

> <span data-ttu-id="13b38-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="13b38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13b38-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="13b38-105">OMA Settings String definition.</span></span>

<span data-ttu-id="13b38-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13b38-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13b38-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="13b38-107">Properties</span></span>
|<span data-ttu-id="13b38-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="13b38-108">Property</span></span>|<span data-ttu-id="13b38-109">Тип</span><span class="sxs-lookup"><span data-stu-id="13b38-109">Type</span></span>|<span data-ttu-id="13b38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13b38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b38-111">displayName</span><span class="sxs-lookup"><span data-stu-id="13b38-111">displayName</span></span>|<span data-ttu-id="13b38-112">String</span><span class="sxs-lookup"><span data-stu-id="13b38-112">String</span></span>|<span data-ttu-id="13b38-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="13b38-113">Display Name.</span></span> <span data-ttu-id="13b38-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13b38-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13b38-115">описание</span><span class="sxs-lookup"><span data-stu-id="13b38-115">description</span></span>|<span data-ttu-id="13b38-116">String</span><span class="sxs-lookup"><span data-stu-id="13b38-116">String</span></span>|<span data-ttu-id="13b38-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="13b38-117">Description.</span></span> <span data-ttu-id="13b38-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13b38-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13b38-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="13b38-119">omaUri</span></span>|<span data-ttu-id="13b38-120">String</span><span class="sxs-lookup"><span data-stu-id="13b38-120">String</span></span>|<span data-ttu-id="13b38-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="13b38-121">OMA.</span></span> <span data-ttu-id="13b38-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13b38-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13b38-123">value</span><span class="sxs-lookup"><span data-stu-id="13b38-123">value</span></span>|<span data-ttu-id="13b38-124">String</span><span class="sxs-lookup"><span data-stu-id="13b38-124">String</span></span>|<span data-ttu-id="13b38-125">Значение</span><span class="sxs-lookup"><span data-stu-id="13b38-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b38-126">Связи</span><span class="sxs-lookup"><span data-stu-id="13b38-126">Relationships</span></span>
<span data-ttu-id="13b38-127">Нет</span><span class="sxs-lookup"><span data-stu-id="13b38-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13b38-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13b38-128">JSON Representation</span></span>
<span data-ttu-id="13b38-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13b38-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



