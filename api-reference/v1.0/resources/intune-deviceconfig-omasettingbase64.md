---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8ab8552205084f41599a37c4a8edf39f329d85d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028044"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="38c4d-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="38c4d-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="38c4d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38c4d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38c4d-105">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="38c4d-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="38c4d-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38c4d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38c4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="38c4d-107">Properties</span></span>
|<span data-ttu-id="38c4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="38c4d-108">Property</span></span>|<span data-ttu-id="38c4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="38c4d-109">Type</span></span>|<span data-ttu-id="38c4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="38c4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38c4d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="38c4d-111">displayName</span></span>|<span data-ttu-id="38c4d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="38c4d-112">String</span></span>|<span data-ttu-id="38c4d-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="38c4d-113">Display Name.</span></span> <span data-ttu-id="38c4d-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38c4d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38c4d-115">description</span><span class="sxs-lookup"><span data-stu-id="38c4d-115">description</span></span>|<span data-ttu-id="38c4d-116">String</span><span class="sxs-lookup"><span data-stu-id="38c4d-116">String</span></span>|<span data-ttu-id="38c4d-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="38c4d-117">Description.</span></span> <span data-ttu-id="38c4d-118">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38c4d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38c4d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="38c4d-119">omaUri</span></span>|<span data-ttu-id="38c4d-120">String</span><span class="sxs-lookup"><span data-stu-id="38c4d-120">String</span></span>|<span data-ttu-id="38c4d-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="38c4d-121">OMA.</span></span> <span data-ttu-id="38c4d-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38c4d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38c4d-123">fileName</span><span class="sxs-lookup"><span data-stu-id="38c4d-123">fileName</span></span>|<span data-ttu-id="38c4d-124">String</span><span class="sxs-lookup"><span data-stu-id="38c4d-124">String</span></span>|<span data-ttu-id="38c4d-125">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="38c4d-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="38c4d-126">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="38c4d-126">\*.crt</span></span> | <span data-ttu-id="38c4d-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="38c4d-127">\*.p7b</span></span> | <span data-ttu-id="38c4d-128">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="38c4d-128">\*.bin).</span></span>|
|<span data-ttu-id="38c4d-129">value</span><span class="sxs-lookup"><span data-stu-id="38c4d-129">value</span></span>|<span data-ttu-id="38c4d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="38c4d-130">String</span></span>|<span data-ttu-id="38c4d-131">Значение</span><span class="sxs-lookup"><span data-stu-id="38c4d-131">Value.</span></span> <span data-ttu-id="38c4d-132">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="38c4d-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="38c4d-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="38c4d-133">Relationships</span></span>
<span data-ttu-id="38c4d-134">Нет</span><span class="sxs-lookup"><span data-stu-id="38c4d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38c4d-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38c4d-135">JSON Representation</span></span>
<span data-ttu-id="38c4d-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38c4d-136">Here is a JSON representation of the resource.</span></span>
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



