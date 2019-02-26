---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258592"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="bde74-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="bde74-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="bde74-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bde74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bde74-105">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="bde74-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="bde74-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bde74-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bde74-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bde74-107">Properties</span></span>
|<span data-ttu-id="bde74-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bde74-108">Property</span></span>|<span data-ttu-id="bde74-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bde74-109">Type</span></span>|<span data-ttu-id="bde74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bde74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bde74-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bde74-111">displayName</span></span>|<span data-ttu-id="bde74-112">String</span><span class="sxs-lookup"><span data-stu-id="bde74-112">String</span></span>|<span data-ttu-id="bde74-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bde74-113">Display Name.</span></span> <span data-ttu-id="bde74-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bde74-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bde74-115">description</span><span class="sxs-lookup"><span data-stu-id="bde74-115">description</span></span>|<span data-ttu-id="bde74-116">String</span><span class="sxs-lookup"><span data-stu-id="bde74-116">String</span></span>|<span data-ttu-id="bde74-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="bde74-117">Description.</span></span> <span data-ttu-id="bde74-118">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bde74-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bde74-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="bde74-119">omaUri</span></span>|<span data-ttu-id="bde74-120">String</span><span class="sxs-lookup"><span data-stu-id="bde74-120">String</span></span>|<span data-ttu-id="bde74-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="bde74-121">OMA.</span></span> <span data-ttu-id="bde74-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bde74-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bde74-123">fileName</span><span class="sxs-lookup"><span data-stu-id="bde74-123">fileName</span></span>|<span data-ttu-id="bde74-124">String</span><span class="sxs-lookup"><span data-stu-id="bde74-124">String</span></span>|<span data-ttu-id="bde74-125">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="bde74-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="bde74-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="bde74-126">\*.crt</span></span> | <span data-ttu-id="bde74-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="bde74-127">\*.p7b</span></span> | <span data-ttu-id="bde74-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="bde74-128">\*.bin).</span></span>|
|<span data-ttu-id="bde74-129">value</span><span class="sxs-lookup"><span data-stu-id="bde74-129">value</span></span>|<span data-ttu-id="bde74-130">Строка</span><span class="sxs-lookup"><span data-stu-id="bde74-130">String</span></span>|<span data-ttu-id="bde74-131">Значение</span><span class="sxs-lookup"><span data-stu-id="bde74-131">Value.</span></span> <span data-ttu-id="bde74-132">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="bde74-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bde74-133">Связи</span><span class="sxs-lookup"><span data-stu-id="bde74-133">Relationships</span></span>
<span data-ttu-id="bde74-134">Нет</span><span class="sxs-lookup"><span data-stu-id="bde74-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bde74-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bde74-135">JSON Representation</span></span>
<span data-ttu-id="bde74-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bde74-136">Here is a JSON representation of the resource.</span></span>
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



