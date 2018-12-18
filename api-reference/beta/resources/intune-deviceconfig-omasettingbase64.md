---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: tfitzmac
ms.openlocfilehash: ee25db94cc1426194166a7c66b9a8a626d62c3e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304076"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="b940e-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="b940e-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="b940e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b940e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b940e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b940e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b940e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b940e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b940e-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="b940e-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="b940e-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b940e-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b940e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b940e-109">Properties</span></span>
|<span data-ttu-id="b940e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b940e-110">Property</span></span>|<span data-ttu-id="b940e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b940e-111">Type</span></span>|<span data-ttu-id="b940e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b940e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b940e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b940e-113">displayName</span></span>|<span data-ttu-id="b940e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b940e-114">String</span></span>|<span data-ttu-id="b940e-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b940e-115">Display Name.</span></span> <span data-ttu-id="b940e-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b940e-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b940e-117">описание</span><span class="sxs-lookup"><span data-stu-id="b940e-117">description</span></span>|<span data-ttu-id="b940e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b940e-118">String</span></span>|<span data-ttu-id="b940e-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="b940e-119">Description.</span></span> <span data-ttu-id="b940e-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b940e-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b940e-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b940e-121">omaUri</span></span>|<span data-ttu-id="b940e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="b940e-122">String</span></span>|<span data-ttu-id="b940e-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="b940e-123">OMA.</span></span> <span data-ttu-id="b940e-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b940e-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b940e-125">fileName</span><span class="sxs-lookup"><span data-stu-id="b940e-125">fileName</span></span>|<span data-ttu-id="b940e-126">String</span><span class="sxs-lookup"><span data-stu-id="b940e-126">String</span></span>|<span data-ttu-id="b940e-127">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="b940e-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="b940e-128">\*.CRT</span><span class="sxs-lookup"><span data-stu-id="b940e-128">\*.crt</span></span> | <span data-ttu-id="b940e-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="b940e-129">\*.p7b</span></span> | <span data-ttu-id="b940e-130">\* .bin).</span><span class="sxs-lookup"><span data-stu-id="b940e-130">\*.bin).</span></span>|
|<span data-ttu-id="b940e-131">value</span><span class="sxs-lookup"><span data-stu-id="b940e-131">value</span></span>|<span data-ttu-id="b940e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b940e-132">String</span></span>|<span data-ttu-id="b940e-133">Значение</span><span class="sxs-lookup"><span data-stu-id="b940e-133">Value.</span></span> <span data-ttu-id="b940e-134">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="b940e-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b940e-135">Связи</span><span class="sxs-lookup"><span data-stu-id="b940e-135">Relationships</span></span>
<span data-ttu-id="b940e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="b940e-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b940e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b940e-137">JSON Representation</span></span>
<span data-ttu-id="b940e-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b940e-138">Here is a JSON representation of the resource.</span></span>
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





