---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2acf41d36b4a664166dc2b5ceeb17dc0b6db4495
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949845"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="668b5-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="668b5-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="668b5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="668b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="668b5-105">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="668b5-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="668b5-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="668b5-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="668b5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="668b5-107">Properties</span></span>
|<span data-ttu-id="668b5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="668b5-108">Property</span></span>|<span data-ttu-id="668b5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="668b5-109">Type</span></span>|<span data-ttu-id="668b5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="668b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="668b5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="668b5-111">displayName</span></span>|<span data-ttu-id="668b5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="668b5-112">String</span></span>|<span data-ttu-id="668b5-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="668b5-113">Display Name.</span></span> <span data-ttu-id="668b5-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="668b5-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="668b5-115">описание</span><span class="sxs-lookup"><span data-stu-id="668b5-115">description</span></span>|<span data-ttu-id="668b5-116">Строка</span><span class="sxs-lookup"><span data-stu-id="668b5-116">String</span></span>|<span data-ttu-id="668b5-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="668b5-117">Description.</span></span> <span data-ttu-id="668b5-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="668b5-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="668b5-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="668b5-119">omaUri</span></span>|<span data-ttu-id="668b5-120">Строка</span><span class="sxs-lookup"><span data-stu-id="668b5-120">String</span></span>|<span data-ttu-id="668b5-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="668b5-121">OMA.</span></span> <span data-ttu-id="668b5-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="668b5-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="668b5-123">fileName</span><span class="sxs-lookup"><span data-stu-id="668b5-123">fileName</span></span>|<span data-ttu-id="668b5-124">String</span><span class="sxs-lookup"><span data-stu-id="668b5-124">String</span></span>|<span data-ttu-id="668b5-125">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="668b5-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="668b5-126">\*.CRT</span><span class="sxs-lookup"><span data-stu-id="668b5-126">\*.crt</span></span> | <span data-ttu-id="668b5-127">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="668b5-127">\*.p7b</span></span> | <span data-ttu-id="668b5-128">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="668b5-128">\*.bin).</span></span>|
|<span data-ttu-id="668b5-129">value</span><span class="sxs-lookup"><span data-stu-id="668b5-129">value</span></span>|<span data-ttu-id="668b5-130">Строка</span><span class="sxs-lookup"><span data-stu-id="668b5-130">String</span></span>|<span data-ttu-id="668b5-131">Значение</span><span class="sxs-lookup"><span data-stu-id="668b5-131">Value.</span></span> <span data-ttu-id="668b5-132">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="668b5-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="668b5-133">Связи</span><span class="sxs-lookup"><span data-stu-id="668b5-133">Relationships</span></span>
<span data-ttu-id="668b5-134">Нет</span><span class="sxs-lookup"><span data-stu-id="668b5-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="668b5-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="668b5-135">JSON Representation</span></span>
<span data-ttu-id="668b5-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668b5-136">Here is a JSON representation of the resource.</span></span>
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



