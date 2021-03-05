---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6288803dd87afa7fe45525c20258bdded34482ea
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470755"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c3070-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="c3070-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="c3070-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3070-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3070-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3070-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3070-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="c3070-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="c3070-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3070-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3070-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3070-108">Properties</span></span>
|<span data-ttu-id="c3070-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3070-109">Property</span></span>|<span data-ttu-id="c3070-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3070-110">Type</span></span>|<span data-ttu-id="c3070-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3070-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3070-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c3070-112">displayName</span></span>|<span data-ttu-id="c3070-113">String</span><span class="sxs-lookup"><span data-stu-id="c3070-113">String</span></span>|<span data-ttu-id="c3070-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c3070-114">Display Name.</span></span> <span data-ttu-id="c3070-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3070-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3070-116">description</span><span class="sxs-lookup"><span data-stu-id="c3070-116">description</span></span>|<span data-ttu-id="c3070-117">String</span><span class="sxs-lookup"><span data-stu-id="c3070-117">String</span></span>|<span data-ttu-id="c3070-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="c3070-118">Description.</span></span> <span data-ttu-id="c3070-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3070-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3070-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="c3070-120">omaUri</span></span>|<span data-ttu-id="c3070-121">String</span><span class="sxs-lookup"><span data-stu-id="c3070-121">String</span></span>|<span data-ttu-id="c3070-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="c3070-122">OMA.</span></span> <span data-ttu-id="c3070-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c3070-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c3070-124">fileName</span><span class="sxs-lookup"><span data-stu-id="c3070-124">fileName</span></span>|<span data-ttu-id="c3070-125">String</span><span class="sxs-lookup"><span data-stu-id="c3070-125">String</span></span>|<span data-ttu-id="c3070-126">Имя файла, связанное с свойством Value (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span><span class="sxs-lookup"><span data-stu-id="c3070-126">File name associated with the Value property (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span></span>|
|<span data-ttu-id="c3070-127">value</span><span class="sxs-lookup"><span data-stu-id="c3070-127">value</span></span>|<span data-ttu-id="c3070-128">String</span><span class="sxs-lookup"><span data-stu-id="c3070-128">String</span></span>|<span data-ttu-id="c3070-129">Значение</span><span class="sxs-lookup"><span data-stu-id="c3070-129">Value.</span></span> <span data-ttu-id="c3070-130">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="c3070-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3070-131">Связи</span><span class="sxs-lookup"><span data-stu-id="c3070-131">Relationships</span></span>
<span data-ttu-id="c3070-132">Нет</span><span class="sxs-lookup"><span data-stu-id="c3070-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3070-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3070-133">JSON Representation</span></span>
<span data-ttu-id="c3070-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3070-134">Here is a JSON representation of the resource.</span></span>
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









