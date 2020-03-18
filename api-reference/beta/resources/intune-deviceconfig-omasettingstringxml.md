---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37c8996eb59186d8b8d5c0c486d40a7b06ce2dc5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788431"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="76664-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="76664-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="76664-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76664-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76664-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76664-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76664-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="76664-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="76664-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76664-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76664-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="76664-108">Properties</span></span>
|<span data-ttu-id="76664-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="76664-109">Property</span></span>|<span data-ttu-id="76664-110">Тип</span><span class="sxs-lookup"><span data-stu-id="76664-110">Type</span></span>|<span data-ttu-id="76664-111">Описание</span><span class="sxs-lookup"><span data-stu-id="76664-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76664-112">displayName</span><span class="sxs-lookup"><span data-stu-id="76664-112">displayName</span></span>|<span data-ttu-id="76664-113">Строка</span><span class="sxs-lookup"><span data-stu-id="76664-113">String</span></span>|<span data-ttu-id="76664-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="76664-114">Display Name.</span></span> <span data-ttu-id="76664-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76664-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76664-116">description</span><span class="sxs-lookup"><span data-stu-id="76664-116">description</span></span>|<span data-ttu-id="76664-117">String</span><span class="sxs-lookup"><span data-stu-id="76664-117">String</span></span>|<span data-ttu-id="76664-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="76664-118">Description.</span></span> <span data-ttu-id="76664-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76664-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76664-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="76664-120">omaUri</span></span>|<span data-ttu-id="76664-121">Строка</span><span class="sxs-lookup"><span data-stu-id="76664-121">String</span></span>|<span data-ttu-id="76664-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="76664-122">OMA.</span></span> <span data-ttu-id="76664-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="76664-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="76664-124">fileName</span><span class="sxs-lookup"><span data-stu-id="76664-124">fileName</span></span>|<span data-ttu-id="76664-125">String</span><span class="sxs-lookup"><span data-stu-id="76664-125">String</span></span>|<span data-ttu-id="76664-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="76664-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="76664-127">value</span><span class="sxs-lookup"><span data-stu-id="76664-127">value</span></span>|<span data-ttu-id="76664-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="76664-128">Binary</span></span>|<span data-ttu-id="76664-129">Значение</span><span class="sxs-lookup"><span data-stu-id="76664-129">Value.</span></span> <span data-ttu-id="76664-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="76664-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="76664-131">Связи</span><span class="sxs-lookup"><span data-stu-id="76664-131">Relationships</span></span>
<span data-ttu-id="76664-132">Нет</span><span class="sxs-lookup"><span data-stu-id="76664-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76664-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76664-133">JSON Representation</span></span>
<span data-ttu-id="76664-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76664-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



