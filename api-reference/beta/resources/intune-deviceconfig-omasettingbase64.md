---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f5b21705d4cabedc24009df794d958c6187af473
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869820"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="24d65-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="24d65-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="24d65-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24d65-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24d65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24d65-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="24d65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24d65-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="24d65-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="24d65-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="24d65-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24d65-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24d65-109">Properties</span></span>
|<span data-ttu-id="24d65-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24d65-110">Property</span></span>|<span data-ttu-id="24d65-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24d65-111">Type</span></span>|<span data-ttu-id="24d65-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24d65-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24d65-113">displayName</span><span class="sxs-lookup"><span data-stu-id="24d65-113">displayName</span></span>|<span data-ttu-id="24d65-114">Строка</span><span class="sxs-lookup"><span data-stu-id="24d65-114">String</span></span>|<span data-ttu-id="24d65-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="24d65-115">Display Name.</span></span> <span data-ttu-id="24d65-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="24d65-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24d65-117">описание</span><span class="sxs-lookup"><span data-stu-id="24d65-117">description</span></span>|<span data-ttu-id="24d65-118">Строка</span><span class="sxs-lookup"><span data-stu-id="24d65-118">String</span></span>|<span data-ttu-id="24d65-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="24d65-119">Description.</span></span> <span data-ttu-id="24d65-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="24d65-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24d65-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="24d65-121">omaUri</span></span>|<span data-ttu-id="24d65-122">Строка</span><span class="sxs-lookup"><span data-stu-id="24d65-122">String</span></span>|<span data-ttu-id="24d65-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="24d65-123">OMA.</span></span> <span data-ttu-id="24d65-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="24d65-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24d65-125">fileName</span><span class="sxs-lookup"><span data-stu-id="24d65-125">fileName</span></span>|<span data-ttu-id="24d65-126">String</span><span class="sxs-lookup"><span data-stu-id="24d65-126">String</span></span>|<span data-ttu-id="24d65-127">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="24d65-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="24d65-128">\*.CRT</span><span class="sxs-lookup"><span data-stu-id="24d65-128">\*.crt</span></span> | <span data-ttu-id="24d65-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="24d65-129">\*.p7b</span></span> | <span data-ttu-id="24d65-130">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="24d65-130">\*.bin).</span></span>|
|<span data-ttu-id="24d65-131">value</span><span class="sxs-lookup"><span data-stu-id="24d65-131">value</span></span>|<span data-ttu-id="24d65-132">Строка</span><span class="sxs-lookup"><span data-stu-id="24d65-132">String</span></span>|<span data-ttu-id="24d65-133">Значение</span><span class="sxs-lookup"><span data-stu-id="24d65-133">Value.</span></span> <span data-ttu-id="24d65-134">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="24d65-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="24d65-135">Связи</span><span class="sxs-lookup"><span data-stu-id="24d65-135">Relationships</span></span>
<span data-ttu-id="24d65-136">Нет</span><span class="sxs-lookup"><span data-stu-id="24d65-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24d65-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24d65-137">JSON Representation</span></span>
<span data-ttu-id="24d65-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24d65-138">Here is a JSON representation of the resource.</span></span>
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





