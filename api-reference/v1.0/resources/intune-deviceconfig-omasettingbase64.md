---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
ms.openlocfilehash: 891c13a4cfcc8c0cf378cb5c7f9c6449bd876b7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027016"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="7f395-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="7f395-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="7f395-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f395-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f395-105">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="7f395-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="7f395-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f395-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f395-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f395-107">Properties</span></span>
|<span data-ttu-id="7f395-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f395-108">Property</span></span>|<span data-ttu-id="7f395-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f395-109">Type</span></span>|<span data-ttu-id="7f395-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f395-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f395-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7f395-111">displayName</span></span>|<span data-ttu-id="7f395-112">String</span><span class="sxs-lookup"><span data-stu-id="7f395-112">String</span></span>|<span data-ttu-id="7f395-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="7f395-113">Display Name.</span></span> <span data-ttu-id="7f395-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f395-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f395-115">описание</span><span class="sxs-lookup"><span data-stu-id="7f395-115">description</span></span>|<span data-ttu-id="7f395-116">String</span><span class="sxs-lookup"><span data-stu-id="7f395-116">String</span></span>|<span data-ttu-id="7f395-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="7f395-117">Description.</span></span> <span data-ttu-id="7f395-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f395-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f395-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="7f395-119">omaUri</span></span>|<span data-ttu-id="7f395-120">String</span><span class="sxs-lookup"><span data-stu-id="7f395-120">String</span></span>|<span data-ttu-id="7f395-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="7f395-121">OMA.</span></span> <span data-ttu-id="7f395-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="7f395-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f395-123">fileName</span><span class="sxs-lookup"><span data-stu-id="7f395-123">fileName</span></span>|<span data-ttu-id="7f395-124">String</span><span class="sxs-lookup"><span data-stu-id="7f395-124">String</span></span>|<span data-ttu-id="7f395-125">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="7f395-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="7f395-126">\*.CRT</span><span class="sxs-lookup"><span data-stu-id="7f395-126">\*.crt</span></span> | <span data-ttu-id="7f395-127">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="7f395-127">\*.p7b</span></span> | <span data-ttu-id="7f395-128">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="7f395-128">\*.bin).</span></span>|
|<span data-ttu-id="7f395-129">value</span><span class="sxs-lookup"><span data-stu-id="7f395-129">value</span></span>|<span data-ttu-id="7f395-130">String</span><span class="sxs-lookup"><span data-stu-id="7f395-130">String</span></span>|<span data-ttu-id="7f395-131">Значение</span><span class="sxs-lookup"><span data-stu-id="7f395-131">Value.</span></span> <span data-ttu-id="7f395-132">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="7f395-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f395-133">Связи</span><span class="sxs-lookup"><span data-stu-id="7f395-133">Relationships</span></span>
<span data-ttu-id="7f395-134">Нет</span><span class="sxs-lookup"><span data-stu-id="7f395-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f395-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f395-135">JSON Representation</span></span>
<span data-ttu-id="7f395-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f395-136">Here is a JSON representation of the resource.</span></span>
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



