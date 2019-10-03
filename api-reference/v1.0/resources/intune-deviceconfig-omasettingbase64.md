---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3986bcb6294e2a6da8240e1f1930778fabbeff4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366582"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="48f87-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="48f87-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="48f87-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48f87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f87-105">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="48f87-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="48f87-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="48f87-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48f87-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="48f87-107">Properties</span></span>
|<span data-ttu-id="48f87-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f87-108">Property</span></span>|<span data-ttu-id="48f87-109">Тип</span><span class="sxs-lookup"><span data-stu-id="48f87-109">Type</span></span>|<span data-ttu-id="48f87-110">Описание</span><span class="sxs-lookup"><span data-stu-id="48f87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f87-111">displayName</span><span class="sxs-lookup"><span data-stu-id="48f87-111">displayName</span></span>|<span data-ttu-id="48f87-112">Строка</span><span class="sxs-lookup"><span data-stu-id="48f87-112">String</span></span>|<span data-ttu-id="48f87-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="48f87-113">Display Name.</span></span> <span data-ttu-id="48f87-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="48f87-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="48f87-115">description</span><span class="sxs-lookup"><span data-stu-id="48f87-115">description</span></span>|<span data-ttu-id="48f87-116">String</span><span class="sxs-lookup"><span data-stu-id="48f87-116">String</span></span>|<span data-ttu-id="48f87-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="48f87-117">Description.</span></span> <span data-ttu-id="48f87-118">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="48f87-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="48f87-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="48f87-119">omaUri</span></span>|<span data-ttu-id="48f87-120">String</span><span class="sxs-lookup"><span data-stu-id="48f87-120">String</span></span>|<span data-ttu-id="48f87-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="48f87-121">OMA.</span></span> <span data-ttu-id="48f87-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="48f87-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="48f87-123">fileName</span><span class="sxs-lookup"><span data-stu-id="48f87-123">fileName</span></span>|<span data-ttu-id="48f87-124">String</span><span class="sxs-lookup"><span data-stu-id="48f87-124">String</span></span>|<span data-ttu-id="48f87-125">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="48f87-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="48f87-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="48f87-126">\*.crt</span></span> | <span data-ttu-id="48f87-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="48f87-127">\*.p7b</span></span> | <span data-ttu-id="48f87-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="48f87-128">\*.bin).</span></span>|
|<span data-ttu-id="48f87-129">value</span><span class="sxs-lookup"><span data-stu-id="48f87-129">value</span></span>|<span data-ttu-id="48f87-130">Строка</span><span class="sxs-lookup"><span data-stu-id="48f87-130">String</span></span>|<span data-ttu-id="48f87-131">Значение</span><span class="sxs-lookup"><span data-stu-id="48f87-131">Value.</span></span> <span data-ttu-id="48f87-132">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="48f87-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f87-133">Связи</span><span class="sxs-lookup"><span data-stu-id="48f87-133">Relationships</span></span>
<span data-ttu-id="48f87-134">Нет</span><span class="sxs-lookup"><span data-stu-id="48f87-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48f87-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48f87-135">JSON Representation</span></span>
<span data-ttu-id="48f87-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48f87-136">Here is a JSON representation of the resource.</span></span>
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




