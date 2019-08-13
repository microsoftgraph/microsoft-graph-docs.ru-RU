---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 502035f3489e86475f12b2e277db3da431b6099e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368529"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="47282-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="47282-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="47282-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47282-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47282-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47282-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47282-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="47282-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="47282-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47282-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47282-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47282-108">Properties</span></span>
|<span data-ttu-id="47282-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47282-109">Property</span></span>|<span data-ttu-id="47282-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47282-110">Type</span></span>|<span data-ttu-id="47282-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47282-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47282-112">displayName</span><span class="sxs-lookup"><span data-stu-id="47282-112">displayName</span></span>|<span data-ttu-id="47282-113">Строка</span><span class="sxs-lookup"><span data-stu-id="47282-113">String</span></span>|<span data-ttu-id="47282-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="47282-114">Display Name.</span></span> <span data-ttu-id="47282-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47282-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47282-116">description</span><span class="sxs-lookup"><span data-stu-id="47282-116">description</span></span>|<span data-ttu-id="47282-117">String</span><span class="sxs-lookup"><span data-stu-id="47282-117">String</span></span>|<span data-ttu-id="47282-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="47282-118">Description.</span></span> <span data-ttu-id="47282-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47282-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47282-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="47282-120">omaUri</span></span>|<span data-ttu-id="47282-121">String</span><span class="sxs-lookup"><span data-stu-id="47282-121">String</span></span>|<span data-ttu-id="47282-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="47282-122">OMA.</span></span> <span data-ttu-id="47282-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47282-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47282-124">fileName</span><span class="sxs-lookup"><span data-stu-id="47282-124">fileName</span></span>|<span data-ttu-id="47282-125">String</span><span class="sxs-lookup"><span data-stu-id="47282-125">String</span></span>|<span data-ttu-id="47282-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="47282-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="47282-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="47282-127">\*.crt</span></span> | <span data-ttu-id="47282-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="47282-128">\*.p7b</span></span> | <span data-ttu-id="47282-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="47282-129">\*.bin).</span></span>|
|<span data-ttu-id="47282-130">value</span><span class="sxs-lookup"><span data-stu-id="47282-130">value</span></span>|<span data-ttu-id="47282-131">Строка</span><span class="sxs-lookup"><span data-stu-id="47282-131">String</span></span>|<span data-ttu-id="47282-132">Значение</span><span class="sxs-lookup"><span data-stu-id="47282-132">Value.</span></span> <span data-ttu-id="47282-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="47282-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="47282-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="47282-134">Relationships</span></span>
<span data-ttu-id="47282-135">Нет</span><span class="sxs-lookup"><span data-stu-id="47282-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47282-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47282-136">JSON Representation</span></span>
<span data-ttu-id="47282-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47282-137">Here is a JSON representation of the resource.</span></span>
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



