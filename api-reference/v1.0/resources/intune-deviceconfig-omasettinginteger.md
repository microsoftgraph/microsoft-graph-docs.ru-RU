---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
ms.openlocfilehash: 36c22b423161d9f3c58c3085fb7b040c663d460b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027897"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="98b34-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="98b34-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="98b34-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98b34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98b34-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="98b34-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="98b34-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="98b34-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98b34-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="98b34-107">Properties</span></span>
|<span data-ttu-id="98b34-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b34-108">Property</span></span>|<span data-ttu-id="98b34-109">Тип</span><span class="sxs-lookup"><span data-stu-id="98b34-109">Type</span></span>|<span data-ttu-id="98b34-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98b34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b34-111">displayName</span><span class="sxs-lookup"><span data-stu-id="98b34-111">displayName</span></span>|<span data-ttu-id="98b34-112">String</span><span class="sxs-lookup"><span data-stu-id="98b34-112">String</span></span>|<span data-ttu-id="98b34-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="98b34-113">Display Name.</span></span> <span data-ttu-id="98b34-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="98b34-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98b34-115">описание</span><span class="sxs-lookup"><span data-stu-id="98b34-115">description</span></span>|<span data-ttu-id="98b34-116">String</span><span class="sxs-lookup"><span data-stu-id="98b34-116">String</span></span>|<span data-ttu-id="98b34-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="98b34-117">Description.</span></span> <span data-ttu-id="98b34-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="98b34-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98b34-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="98b34-119">omaUri</span></span>|<span data-ttu-id="98b34-120">String</span><span class="sxs-lookup"><span data-stu-id="98b34-120">String</span></span>|<span data-ttu-id="98b34-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="98b34-121">OMA.</span></span> <span data-ttu-id="98b34-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="98b34-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98b34-123">value</span><span class="sxs-lookup"><span data-stu-id="98b34-123">value</span></span>|<span data-ttu-id="98b34-124">Int32</span><span class="sxs-lookup"><span data-stu-id="98b34-124">Int32</span></span>|<span data-ttu-id="98b34-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="98b34-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98b34-126">Связи</span><span class="sxs-lookup"><span data-stu-id="98b34-126">Relationships</span></span>
<span data-ttu-id="98b34-127">Нет</span><span class="sxs-lookup"><span data-stu-id="98b34-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98b34-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98b34-128">JSON Representation</span></span>
<span data-ttu-id="98b34-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98b34-129">Here is a JSON representation of the resource.</span></span>
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



