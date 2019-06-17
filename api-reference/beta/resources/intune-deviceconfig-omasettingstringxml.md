---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee1f412ad21ece1f103b71281b33f1ea41b6dc9a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987938"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="e3208-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="e3208-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="e3208-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3208-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3208-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3208-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3208-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="e3208-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="e3208-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3208-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3208-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3208-108">Properties</span></span>
|<span data-ttu-id="e3208-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3208-109">Property</span></span>|<span data-ttu-id="e3208-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3208-110">Type</span></span>|<span data-ttu-id="e3208-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3208-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3208-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e3208-112">displayName</span></span>|<span data-ttu-id="e3208-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e3208-113">String</span></span>|<span data-ttu-id="e3208-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e3208-114">Display Name.</span></span> <span data-ttu-id="e3208-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3208-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3208-116">description</span><span class="sxs-lookup"><span data-stu-id="e3208-116">description</span></span>|<span data-ttu-id="e3208-117">String</span><span class="sxs-lookup"><span data-stu-id="e3208-117">String</span></span>|<span data-ttu-id="e3208-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="e3208-118">Description.</span></span> <span data-ttu-id="e3208-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3208-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3208-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="e3208-120">omaUri</span></span>|<span data-ttu-id="e3208-121">Строка</span><span class="sxs-lookup"><span data-stu-id="e3208-121">String</span></span>|<span data-ttu-id="e3208-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="e3208-122">OMA.</span></span> <span data-ttu-id="e3208-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e3208-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e3208-124">fileName</span><span class="sxs-lookup"><span data-stu-id="e3208-124">fileName</span></span>|<span data-ttu-id="e3208-125">String</span><span class="sxs-lookup"><span data-stu-id="e3208-125">String</span></span>|<span data-ttu-id="e3208-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="e3208-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="e3208-127">value</span><span class="sxs-lookup"><span data-stu-id="e3208-127">value</span></span>|<span data-ttu-id="e3208-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="e3208-128">Binary</span></span>|<span data-ttu-id="e3208-129">Значение</span><span class="sxs-lookup"><span data-stu-id="e3208-129">Value.</span></span> <span data-ttu-id="e3208-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="e3208-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3208-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="e3208-131">Relationships</span></span>
<span data-ttu-id="e3208-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e3208-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3208-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3208-133">JSON Representation</span></span>
<span data-ttu-id="e3208-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3208-134">Here is a JSON representation of the resource.</span></span>
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





