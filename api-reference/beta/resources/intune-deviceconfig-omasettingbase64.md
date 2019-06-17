---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ecb77bc317216e77cb53c31b8be9bded9cafc19
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995555"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="bca7e-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="bca7e-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="bca7e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca7e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bca7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca7e-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="bca7e-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="bca7e-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bca7e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bca7e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bca7e-108">Properties</span></span>
|<span data-ttu-id="bca7e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bca7e-109">Property</span></span>|<span data-ttu-id="bca7e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bca7e-110">Type</span></span>|<span data-ttu-id="bca7e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bca7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca7e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bca7e-112">displayName</span></span>|<span data-ttu-id="bca7e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bca7e-113">String</span></span>|<span data-ttu-id="bca7e-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bca7e-114">Display Name.</span></span> <span data-ttu-id="bca7e-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bca7e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bca7e-116">description</span><span class="sxs-lookup"><span data-stu-id="bca7e-116">description</span></span>|<span data-ttu-id="bca7e-117">String</span><span class="sxs-lookup"><span data-stu-id="bca7e-117">String</span></span>|<span data-ttu-id="bca7e-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="bca7e-118">Description.</span></span> <span data-ttu-id="bca7e-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bca7e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bca7e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="bca7e-120">omaUri</span></span>|<span data-ttu-id="bca7e-121">String</span><span class="sxs-lookup"><span data-stu-id="bca7e-121">String</span></span>|<span data-ttu-id="bca7e-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="bca7e-122">OMA.</span></span> <span data-ttu-id="bca7e-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bca7e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bca7e-124">fileName</span><span class="sxs-lookup"><span data-stu-id="bca7e-124">fileName</span></span>|<span data-ttu-id="bca7e-125">String</span><span class="sxs-lookup"><span data-stu-id="bca7e-125">String</span></span>|<span data-ttu-id="bca7e-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="bca7e-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="bca7e-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="bca7e-127">\*.crt</span></span> | <span data-ttu-id="bca7e-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="bca7e-128">\*.p7b</span></span> | <span data-ttu-id="bca7e-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="bca7e-129">\*.bin).</span></span>|
|<span data-ttu-id="bca7e-130">value</span><span class="sxs-lookup"><span data-stu-id="bca7e-130">value</span></span>|<span data-ttu-id="bca7e-131">Строка</span><span class="sxs-lookup"><span data-stu-id="bca7e-131">String</span></span>|<span data-ttu-id="bca7e-132">Значение</span><span class="sxs-lookup"><span data-stu-id="bca7e-132">Value.</span></span> <span data-ttu-id="bca7e-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="bca7e-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca7e-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="bca7e-134">Relationships</span></span>
<span data-ttu-id="bca7e-135">Нет</span><span class="sxs-lookup"><span data-stu-id="bca7e-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bca7e-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bca7e-136">JSON Representation</span></span>
<span data-ttu-id="bca7e-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bca7e-137">Here is a JSON representation of the resource.</span></span>
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





