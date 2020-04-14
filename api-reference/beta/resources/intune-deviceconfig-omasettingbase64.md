---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f5089c40e2c79d0a3a2e9a920de10d8e5eb4bc1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402007"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e10b1-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="e10b1-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="e10b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e10b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e10b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e10b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e10b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10b1-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="e10b1-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e10b1-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10b1-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e10b1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e10b1-109">Properties</span></span>
|<span data-ttu-id="e10b1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e10b1-110">Property</span></span>|<span data-ttu-id="e10b1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e10b1-111">Type</span></span>|<span data-ttu-id="e10b1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e10b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10b1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e10b1-113">displayName</span></span>|<span data-ttu-id="e10b1-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e10b1-114">String</span></span>|<span data-ttu-id="e10b1-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e10b1-115">Display Name.</span></span> <span data-ttu-id="e10b1-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10b1-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10b1-117">description</span><span class="sxs-lookup"><span data-stu-id="e10b1-117">description</span></span>|<span data-ttu-id="e10b1-118">String</span><span class="sxs-lookup"><span data-stu-id="e10b1-118">String</span></span>|<span data-ttu-id="e10b1-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="e10b1-119">Description.</span></span> <span data-ttu-id="e10b1-120">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10b1-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10b1-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="e10b1-121">omaUri</span></span>|<span data-ttu-id="e10b1-122">String</span><span class="sxs-lookup"><span data-stu-id="e10b1-122">String</span></span>|<span data-ttu-id="e10b1-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="e10b1-123">OMA.</span></span> <span data-ttu-id="e10b1-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10b1-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10b1-125">fileName</span><span class="sxs-lookup"><span data-stu-id="e10b1-125">fileName</span></span>|<span data-ttu-id="e10b1-126">String</span><span class="sxs-lookup"><span data-stu-id="e10b1-126">String</span></span>|<span data-ttu-id="e10b1-127">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="e10b1-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e10b1-128">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="e10b1-128">\*.crt</span></span> | <span data-ttu-id="e10b1-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="e10b1-129">\*.p7b</span></span> | <span data-ttu-id="e10b1-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="e10b1-130">\*.bin).</span></span>|
|<span data-ttu-id="e10b1-131">value</span><span class="sxs-lookup"><span data-stu-id="e10b1-131">value</span></span>|<span data-ttu-id="e10b1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e10b1-132">String</span></span>|<span data-ttu-id="e10b1-133">Значение</span><span class="sxs-lookup"><span data-stu-id="e10b1-133">Value.</span></span> <span data-ttu-id="e10b1-134">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="e10b1-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10b1-135">Связи</span><span class="sxs-lookup"><span data-stu-id="e10b1-135">Relationships</span></span>
<span data-ttu-id="e10b1-136">Нет</span><span class="sxs-lookup"><span data-stu-id="e10b1-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e10b1-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e10b1-137">JSON Representation</span></span>
<span data-ttu-id="e10b1-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e10b1-138">Here is a JSON representation of the resource.</span></span>
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



