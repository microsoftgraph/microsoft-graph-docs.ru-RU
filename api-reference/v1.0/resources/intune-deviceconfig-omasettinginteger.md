---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cf2e556fe434a7a0ab8baa4d42a4098e66c698cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473006"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="05e33-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="05e33-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="05e33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05e33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05e33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05e33-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="05e33-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="05e33-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05e33-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05e33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05e33-108">Properties</span></span>
|<span data-ttu-id="05e33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05e33-109">Property</span></span>|<span data-ttu-id="05e33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05e33-110">Type</span></span>|<span data-ttu-id="05e33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05e33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05e33-112">displayName</span><span class="sxs-lookup"><span data-stu-id="05e33-112">displayName</span></span>|<span data-ttu-id="05e33-113">Строка</span><span class="sxs-lookup"><span data-stu-id="05e33-113">String</span></span>|<span data-ttu-id="05e33-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="05e33-114">Display Name.</span></span> <span data-ttu-id="05e33-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05e33-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05e33-116">description</span><span class="sxs-lookup"><span data-stu-id="05e33-116">description</span></span>|<span data-ttu-id="05e33-117">String</span><span class="sxs-lookup"><span data-stu-id="05e33-117">String</span></span>|<span data-ttu-id="05e33-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="05e33-118">Description.</span></span> <span data-ttu-id="05e33-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05e33-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05e33-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="05e33-120">omaUri</span></span>|<span data-ttu-id="05e33-121">String</span><span class="sxs-lookup"><span data-stu-id="05e33-121">String</span></span>|<span data-ttu-id="05e33-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="05e33-122">OMA.</span></span> <span data-ttu-id="05e33-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05e33-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05e33-124">value</span><span class="sxs-lookup"><span data-stu-id="05e33-124">value</span></span>|<span data-ttu-id="05e33-125">Int32</span><span class="sxs-lookup"><span data-stu-id="05e33-125">Int32</span></span>|<span data-ttu-id="05e33-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="05e33-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05e33-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="05e33-127">Relationships</span></span>
<span data-ttu-id="05e33-128">Нет</span><span class="sxs-lookup"><span data-stu-id="05e33-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05e33-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05e33-129">JSON Representation</span></span>
<span data-ttu-id="05e33-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05e33-130">Here is a JSON representation of the resource.</span></span>
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







