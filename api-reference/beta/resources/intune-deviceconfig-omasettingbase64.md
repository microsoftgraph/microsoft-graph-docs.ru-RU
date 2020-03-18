---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e95f17d0b9e4a8347c71042244100c96590a527
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788480"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="a8d32-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="a8d32-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="a8d32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8d32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8d32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8d32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d32-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="a8d32-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="a8d32-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8d32-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8d32-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8d32-108">Properties</span></span>
|<span data-ttu-id="a8d32-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8d32-109">Property</span></span>|<span data-ttu-id="a8d32-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8d32-110">Type</span></span>|<span data-ttu-id="a8d32-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d32-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a8d32-112">displayName</span></span>|<span data-ttu-id="a8d32-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a8d32-113">String</span></span>|<span data-ttu-id="a8d32-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a8d32-114">Display Name.</span></span> <span data-ttu-id="a8d32-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8d32-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8d32-116">description</span><span class="sxs-lookup"><span data-stu-id="a8d32-116">description</span></span>|<span data-ttu-id="a8d32-117">String</span><span class="sxs-lookup"><span data-stu-id="a8d32-117">String</span></span>|<span data-ttu-id="a8d32-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="a8d32-118">Description.</span></span> <span data-ttu-id="a8d32-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8d32-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8d32-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="a8d32-120">omaUri</span></span>|<span data-ttu-id="a8d32-121">String</span><span class="sxs-lookup"><span data-stu-id="a8d32-121">String</span></span>|<span data-ttu-id="a8d32-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="a8d32-122">OMA.</span></span> <span data-ttu-id="a8d32-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a8d32-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a8d32-124">fileName</span><span class="sxs-lookup"><span data-stu-id="a8d32-124">fileName</span></span>|<span data-ttu-id="a8d32-125">String</span><span class="sxs-lookup"><span data-stu-id="a8d32-125">String</span></span>|<span data-ttu-id="a8d32-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="a8d32-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="a8d32-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="a8d32-127">\*.crt</span></span> | <span data-ttu-id="a8d32-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="a8d32-128">\*.p7b</span></span> | <span data-ttu-id="a8d32-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="a8d32-129">\*.bin).</span></span>|
|<span data-ttu-id="a8d32-130">value</span><span class="sxs-lookup"><span data-stu-id="a8d32-130">value</span></span>|<span data-ttu-id="a8d32-131">Строка</span><span class="sxs-lookup"><span data-stu-id="a8d32-131">String</span></span>|<span data-ttu-id="a8d32-132">Значение</span><span class="sxs-lookup"><span data-stu-id="a8d32-132">Value.</span></span> <span data-ttu-id="a8d32-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="a8d32-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8d32-134">Связи</span><span class="sxs-lookup"><span data-stu-id="a8d32-134">Relationships</span></span>
<span data-ttu-id="a8d32-135">Нет</span><span class="sxs-lookup"><span data-stu-id="a8d32-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8d32-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8d32-136">JSON Representation</span></span>
<span data-ttu-id="a8d32-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8d32-137">Here is a JSON representation of the resource.</span></span>
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



