---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72c7bdd9eda67d9bdebc2452ad778d4ad653d7df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079279"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="3e2b1-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="3e2b1-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="3e2b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e2b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e2b1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e2b1-106">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="3e2b1-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e2b1-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e2b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e2b1-108">Properties</span></span>
|<span data-ttu-id="3e2b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e2b1-109">Property</span></span>|<span data-ttu-id="3e2b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e2b1-110">Type</span></span>|<span data-ttu-id="3e2b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e2b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e2b1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3e2b1-112">displayName</span></span>|<span data-ttu-id="3e2b1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3e2b1-113">String</span></span>|<span data-ttu-id="3e2b1-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-114">Display Name.</span></span> <span data-ttu-id="3e2b1-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e2b1-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e2b1-116">description</span><span class="sxs-lookup"><span data-stu-id="3e2b1-116">description</span></span>|<span data-ttu-id="3e2b1-117">Строка</span><span class="sxs-lookup"><span data-stu-id="3e2b1-117">String</span></span>|<span data-ttu-id="3e2b1-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-118">Description.</span></span> <span data-ttu-id="3e2b1-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e2b1-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e2b1-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3e2b1-120">omaUri</span></span>|<span data-ttu-id="3e2b1-121">String</span><span class="sxs-lookup"><span data-stu-id="3e2b1-121">String</span></span>|<span data-ttu-id="3e2b1-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-122">OMA.</span></span> <span data-ttu-id="3e2b1-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e2b1-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e2b1-124">fileName</span><span class="sxs-lookup"><span data-stu-id="3e2b1-124">fileName</span></span>|<span data-ttu-id="3e2b1-125">String</span><span class="sxs-lookup"><span data-stu-id="3e2b1-125">String</span></span>|<span data-ttu-id="3e2b1-126">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="3e2b1-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="3e2b1-127">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="3e2b1-127">\*.crt</span></span> | <span data-ttu-id="3e2b1-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="3e2b1-128">\*.p7b</span></span> | <span data-ttu-id="3e2b1-129">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="3e2b1-129">\*.bin).</span></span>|
|<span data-ttu-id="3e2b1-130">value</span><span class="sxs-lookup"><span data-stu-id="3e2b1-130">value</span></span>|<span data-ttu-id="3e2b1-131">String</span><span class="sxs-lookup"><span data-stu-id="3e2b1-131">String</span></span>|<span data-ttu-id="3e2b1-132">Значение</span><span class="sxs-lookup"><span data-stu-id="3e2b1-132">Value.</span></span> <span data-ttu-id="3e2b1-133">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="3e2b1-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e2b1-134">Связи</span><span class="sxs-lookup"><span data-stu-id="3e2b1-134">Relationships</span></span>
<span data-ttu-id="3e2b1-135">Нет</span><span class="sxs-lookup"><span data-stu-id="3e2b1-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e2b1-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e2b1-136">JSON Representation</span></span>
<span data-ttu-id="3e2b1-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e2b1-137">Here is a JSON representation of the resource.</span></span>
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









