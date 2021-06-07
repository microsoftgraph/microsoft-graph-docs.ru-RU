---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cfbe888eb5bbe10fc974a91769246d025d284c39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751393"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="fd4fd-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="fd4fd-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="fd4fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd4fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd4fd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd4fd-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="fd4fd-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd4fd-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd4fd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd4fd-108">Properties</span></span>
|<span data-ttu-id="fd4fd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd4fd-109">Property</span></span>|<span data-ttu-id="fd4fd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fd4fd-110">Type</span></span>|<span data-ttu-id="fd4fd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd4fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd4fd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fd4fd-112">displayName</span></span>|<span data-ttu-id="fd4fd-113">String</span><span class="sxs-lookup"><span data-stu-id="fd4fd-113">String</span></span>|<span data-ttu-id="fd4fd-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-114">Display Name.</span></span> <span data-ttu-id="fd4fd-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd4fd-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd4fd-116">description</span><span class="sxs-lookup"><span data-stu-id="fd4fd-116">description</span></span>|<span data-ttu-id="fd4fd-117">String</span><span class="sxs-lookup"><span data-stu-id="fd4fd-117">String</span></span>|<span data-ttu-id="fd4fd-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-118">Description.</span></span> <span data-ttu-id="fd4fd-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd4fd-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd4fd-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fd4fd-120">omaUri</span></span>|<span data-ttu-id="fd4fd-121">String</span><span class="sxs-lookup"><span data-stu-id="fd4fd-121">String</span></span>|<span data-ttu-id="fd4fd-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-122">OMA.</span></span> <span data-ttu-id="fd4fd-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd4fd-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd4fd-124">fileName</span><span class="sxs-lookup"><span data-stu-id="fd4fd-124">fileName</span></span>|<span data-ttu-id="fd4fd-125">String</span><span class="sxs-lookup"><span data-stu-id="fd4fd-125">String</span></span>|<span data-ttu-id="fd4fd-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="fd4fd-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="fd4fd-127">\*.crt</span><span class="sxs-lookup"><span data-stu-id="fd4fd-127">\*.crt</span></span> | <span data-ttu-id="fd4fd-128">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="fd4fd-128">\*.p7b</span></span> | <span data-ttu-id="fd4fd-129">\*.bin).</span><span class="sxs-lookup"><span data-stu-id="fd4fd-129">\*.bin).</span></span>|
|<span data-ttu-id="fd4fd-130">value</span><span class="sxs-lookup"><span data-stu-id="fd4fd-130">value</span></span>|<span data-ttu-id="fd4fd-131">String</span><span class="sxs-lookup"><span data-stu-id="fd4fd-131">String</span></span>|<span data-ttu-id="fd4fd-132">Значение</span><span class="sxs-lookup"><span data-stu-id="fd4fd-132">Value.</span></span> <span data-ttu-id="fd4fd-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="fd4fd-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd4fd-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="fd4fd-134">Relationships</span></span>
<span data-ttu-id="fd4fd-135">Нет</span><span class="sxs-lookup"><span data-stu-id="fd4fd-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd4fd-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd4fd-136">JSON Representation</span></span>
<span data-ttu-id="fd4fd-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd4fd-137">Here is a JSON representation of the resource.</span></span>
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




