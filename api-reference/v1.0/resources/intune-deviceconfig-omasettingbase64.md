---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0958243a84c738dc1c04bde866e535f488dbcd18
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473073"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="beb1b-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="beb1b-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="beb1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="beb1b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="beb1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb1b-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="beb1b-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="beb1b-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="beb1b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="beb1b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="beb1b-108">Properties</span></span>
|<span data-ttu-id="beb1b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="beb1b-109">Property</span></span>|<span data-ttu-id="beb1b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="beb1b-110">Type</span></span>|<span data-ttu-id="beb1b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="beb1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb1b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="beb1b-112">displayName</span></span>|<span data-ttu-id="beb1b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="beb1b-113">String</span></span>|<span data-ttu-id="beb1b-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="beb1b-114">Display Name.</span></span> <span data-ttu-id="beb1b-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="beb1b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="beb1b-116">description</span><span class="sxs-lookup"><span data-stu-id="beb1b-116">description</span></span>|<span data-ttu-id="beb1b-117">String</span><span class="sxs-lookup"><span data-stu-id="beb1b-117">String</span></span>|<span data-ttu-id="beb1b-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="beb1b-118">Description.</span></span> <span data-ttu-id="beb1b-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="beb1b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="beb1b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="beb1b-120">omaUri</span></span>|<span data-ttu-id="beb1b-121">String</span><span class="sxs-lookup"><span data-stu-id="beb1b-121">String</span></span>|<span data-ttu-id="beb1b-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="beb1b-122">OMA.</span></span> <span data-ttu-id="beb1b-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="beb1b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="beb1b-124">fileName</span><span class="sxs-lookup"><span data-stu-id="beb1b-124">fileName</span></span>|<span data-ttu-id="beb1b-125">String</span><span class="sxs-lookup"><span data-stu-id="beb1b-125">String</span></span>|<span data-ttu-id="beb1b-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="beb1b-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="beb1b-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="beb1b-127">\*.crt</span></span> | <span data-ttu-id="beb1b-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="beb1b-128">\*.p7b</span></span> | <span data-ttu-id="beb1b-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="beb1b-129">\*.bin).</span></span>|
|<span data-ttu-id="beb1b-130">value</span><span class="sxs-lookup"><span data-stu-id="beb1b-130">value</span></span>|<span data-ttu-id="beb1b-131">Строка</span><span class="sxs-lookup"><span data-stu-id="beb1b-131">String</span></span>|<span data-ttu-id="beb1b-132">Значение</span><span class="sxs-lookup"><span data-stu-id="beb1b-132">Value.</span></span> <span data-ttu-id="beb1b-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="beb1b-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="beb1b-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="beb1b-134">Relationships</span></span>
<span data-ttu-id="beb1b-135">Нет</span><span class="sxs-lookup"><span data-stu-id="beb1b-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="beb1b-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="beb1b-136">JSON Representation</span></span>
<span data-ttu-id="beb1b-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beb1b-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```







