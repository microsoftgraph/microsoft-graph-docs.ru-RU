---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33488e3b6500056c0f183d5e219e5f5ec489c178
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534880"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="3b418-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="3b418-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="3b418-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b418-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b418-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="3b418-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="3b418-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3b418-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b418-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b418-108">Properties</span></span>
|<span data-ttu-id="3b418-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b418-109">Property</span></span>|<span data-ttu-id="3b418-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3b418-110">Type</span></span>|<span data-ttu-id="3b418-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3b418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b418-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3b418-112">displayName</span></span>|<span data-ttu-id="3b418-113">String</span><span class="sxs-lookup"><span data-stu-id="3b418-113">String</span></span>|<span data-ttu-id="3b418-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3b418-114">Display Name.</span></span> <span data-ttu-id="3b418-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3b418-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3b418-116">description</span><span class="sxs-lookup"><span data-stu-id="3b418-116">description</span></span>|<span data-ttu-id="3b418-117">String</span><span class="sxs-lookup"><span data-stu-id="3b418-117">String</span></span>|<span data-ttu-id="3b418-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="3b418-118">Description.</span></span> <span data-ttu-id="3b418-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3b418-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3b418-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3b418-120">omaUri</span></span>|<span data-ttu-id="3b418-121">String</span><span class="sxs-lookup"><span data-stu-id="3b418-121">String</span></span>|<span data-ttu-id="3b418-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="3b418-122">OMA.</span></span> <span data-ttu-id="3b418-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3b418-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3b418-124">fileName</span><span class="sxs-lookup"><span data-stu-id="3b418-124">fileName</span></span>|<span data-ttu-id="3b418-125">String</span><span class="sxs-lookup"><span data-stu-id="3b418-125">String</span></span>|<span data-ttu-id="3b418-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="3b418-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="3b418-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="3b418-127">\*.crt</span></span> | <span data-ttu-id="3b418-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="3b418-128">\*.p7b</span></span> | <span data-ttu-id="3b418-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="3b418-129">\*.bin).</span></span>|
|<span data-ttu-id="3b418-130">value</span><span class="sxs-lookup"><span data-stu-id="3b418-130">value</span></span>|<span data-ttu-id="3b418-131">Строка</span><span class="sxs-lookup"><span data-stu-id="3b418-131">String</span></span>|<span data-ttu-id="3b418-132">Значение</span><span class="sxs-lookup"><span data-stu-id="3b418-132">Value.</span></span> <span data-ttu-id="3b418-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="3b418-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b418-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="3b418-134">Relationships</span></span>
<span data-ttu-id="3b418-135">Нет</span><span class="sxs-lookup"><span data-stu-id="3b418-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b418-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b418-136">JSON Representation</span></span>
<span data-ttu-id="3b418-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b418-137">Here is a JSON representation of the resource.</span></span>
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





