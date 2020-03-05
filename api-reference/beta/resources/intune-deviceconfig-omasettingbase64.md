---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cba87b6ce02f9683de9e4013585b2a960f8df512
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529571"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="27317-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="27317-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="27317-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="27317-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27317-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27317-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27317-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27317-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27317-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="27317-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="27317-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="27317-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27317-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="27317-109">Properties</span></span>
|<span data-ttu-id="27317-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="27317-110">Property</span></span>|<span data-ttu-id="27317-111">Тип</span><span class="sxs-lookup"><span data-stu-id="27317-111">Type</span></span>|<span data-ttu-id="27317-112">Описание</span><span class="sxs-lookup"><span data-stu-id="27317-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27317-113">displayName</span><span class="sxs-lookup"><span data-stu-id="27317-113">displayName</span></span>|<span data-ttu-id="27317-114">Строка</span><span class="sxs-lookup"><span data-stu-id="27317-114">String</span></span>|<span data-ttu-id="27317-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="27317-115">Display Name.</span></span> <span data-ttu-id="27317-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="27317-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="27317-117">description</span><span class="sxs-lookup"><span data-stu-id="27317-117">description</span></span>|<span data-ttu-id="27317-118">String</span><span class="sxs-lookup"><span data-stu-id="27317-118">String</span></span>|<span data-ttu-id="27317-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="27317-119">Description.</span></span> <span data-ttu-id="27317-120">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="27317-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="27317-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="27317-121">omaUri</span></span>|<span data-ttu-id="27317-122">String</span><span class="sxs-lookup"><span data-stu-id="27317-122">String</span></span>|<span data-ttu-id="27317-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="27317-123">OMA.</span></span> <span data-ttu-id="27317-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="27317-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="27317-125">fileName</span><span class="sxs-lookup"><span data-stu-id="27317-125">fileName</span></span>|<span data-ttu-id="27317-126">String</span><span class="sxs-lookup"><span data-stu-id="27317-126">String</span></span>|<span data-ttu-id="27317-127">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="27317-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="27317-128">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="27317-128">\*.crt</span></span> | <span data-ttu-id="27317-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="27317-129">\*.p7b</span></span> | <span data-ttu-id="27317-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="27317-130">\*.bin).</span></span>|
|<span data-ttu-id="27317-131">value</span><span class="sxs-lookup"><span data-stu-id="27317-131">value</span></span>|<span data-ttu-id="27317-132">Строка</span><span class="sxs-lookup"><span data-stu-id="27317-132">String</span></span>|<span data-ttu-id="27317-133">Значение</span><span class="sxs-lookup"><span data-stu-id="27317-133">Value.</span></span> <span data-ttu-id="27317-134">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="27317-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="27317-135">Связи</span><span class="sxs-lookup"><span data-stu-id="27317-135">Relationships</span></span>
<span data-ttu-id="27317-136">Нет</span><span class="sxs-lookup"><span data-stu-id="27317-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27317-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27317-137">JSON Representation</span></span>
<span data-ttu-id="27317-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27317-138">Here is a JSON representation of the resource.</span></span>
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



