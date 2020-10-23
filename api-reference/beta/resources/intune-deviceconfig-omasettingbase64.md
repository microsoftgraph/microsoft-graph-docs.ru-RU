---
title: Тип ресурса omaSettingBase64
description: Определение параметров OMA в кодировке Base64.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a21ae3f800161b1f5406cdba6c6f9b0de583d1c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722987"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c6f87-103">Тип ресурса omaSettingBase64</span><span class="sxs-lookup"><span data-stu-id="c6f87-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="c6f87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6f87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6f87-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6f87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6f87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6f87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6f87-107">Определение параметров OMA в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="c6f87-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="c6f87-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6f87-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6f87-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6f87-109">Properties</span></span>
|<span data-ttu-id="c6f87-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6f87-110">Property</span></span>|<span data-ttu-id="c6f87-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c6f87-111">Type</span></span>|<span data-ttu-id="c6f87-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c6f87-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6f87-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c6f87-113">displayName</span></span>|<span data-ttu-id="c6f87-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c6f87-114">String</span></span>|<span data-ttu-id="c6f87-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c6f87-115">Display Name.</span></span> <span data-ttu-id="c6f87-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6f87-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c6f87-117">description</span><span class="sxs-lookup"><span data-stu-id="c6f87-117">description</span></span>|<span data-ttu-id="c6f87-118">Строка</span><span class="sxs-lookup"><span data-stu-id="c6f87-118">String</span></span>|<span data-ttu-id="c6f87-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="c6f87-119">Description.</span></span> <span data-ttu-id="c6f87-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6f87-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c6f87-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="c6f87-121">omaUri</span></span>|<span data-ttu-id="c6f87-122">String</span><span class="sxs-lookup"><span data-stu-id="c6f87-122">String</span></span>|<span data-ttu-id="c6f87-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="c6f87-123">OMA.</span></span> <span data-ttu-id="c6f87-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c6f87-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c6f87-125">fileName</span><span class="sxs-lookup"><span data-stu-id="c6f87-125">fileName</span></span>|<span data-ttu-id="c6f87-126">String</span><span class="sxs-lookup"><span data-stu-id="c6f87-126">String</span></span>|<span data-ttu-id="c6f87-127">Имя файла, связанное со свойством Value (CER, </span><span class="sxs-lookup"><span data-stu-id="c6f87-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c6f87-128">\*. CRT</span><span class="sxs-lookup"><span data-stu-id="c6f87-128">\*.crt</span></span> | <span data-ttu-id="c6f87-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="c6f87-129">\*.p7b</span></span> | <span data-ttu-id="c6f87-130">\*. bin).</span><span class="sxs-lookup"><span data-stu-id="c6f87-130">\*.bin).</span></span>|
|<span data-ttu-id="c6f87-131">value</span><span class="sxs-lookup"><span data-stu-id="c6f87-131">value</span></span>|<span data-ttu-id="c6f87-132">String</span><span class="sxs-lookup"><span data-stu-id="c6f87-132">String</span></span>|<span data-ttu-id="c6f87-133">Значение</span><span class="sxs-lookup"><span data-stu-id="c6f87-133">Value.</span></span> <span data-ttu-id="c6f87-134">(строка в кодировке Base64).</span><span class="sxs-lookup"><span data-stu-id="c6f87-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6f87-135">Связи</span><span class="sxs-lookup"><span data-stu-id="c6f87-135">Relationships</span></span>
<span data-ttu-id="c6f87-136">Нет</span><span class="sxs-lookup"><span data-stu-id="c6f87-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6f87-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6f87-137">JSON Representation</span></span>
<span data-ttu-id="c6f87-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6f87-138">Here is a JSON representation of the resource.</span></span>
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





