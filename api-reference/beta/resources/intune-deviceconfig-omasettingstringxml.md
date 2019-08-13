---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ddce8acb059ff28ad37bce284efc6f3fd29f0224
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368445"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="cc02b-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="cc02b-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="cc02b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc02b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc02b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc02b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc02b-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="cc02b-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="cc02b-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cc02b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc02b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc02b-108">Properties</span></span>
|<span data-ttu-id="cc02b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc02b-109">Property</span></span>|<span data-ttu-id="cc02b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cc02b-110">Type</span></span>|<span data-ttu-id="cc02b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc02b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc02b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cc02b-112">displayName</span></span>|<span data-ttu-id="cc02b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="cc02b-113">String</span></span>|<span data-ttu-id="cc02b-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="cc02b-114">Display Name.</span></span> <span data-ttu-id="cc02b-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cc02b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cc02b-116">description</span><span class="sxs-lookup"><span data-stu-id="cc02b-116">description</span></span>|<span data-ttu-id="cc02b-117">String</span><span class="sxs-lookup"><span data-stu-id="cc02b-117">String</span></span>|<span data-ttu-id="cc02b-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="cc02b-118">Description.</span></span> <span data-ttu-id="cc02b-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cc02b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cc02b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="cc02b-120">omaUri</span></span>|<span data-ttu-id="cc02b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="cc02b-121">String</span></span>|<span data-ttu-id="cc02b-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="cc02b-122">OMA.</span></span> <span data-ttu-id="cc02b-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cc02b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cc02b-124">fileName</span><span class="sxs-lookup"><span data-stu-id="cc02b-124">fileName</span></span>|<span data-ttu-id="cc02b-125">String</span><span class="sxs-lookup"><span data-stu-id="cc02b-125">String</span></span>|<span data-ttu-id="cc02b-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="cc02b-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="cc02b-127">value</span><span class="sxs-lookup"><span data-stu-id="cc02b-127">value</span></span>|<span data-ttu-id="cc02b-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="cc02b-128">Binary</span></span>|<span data-ttu-id="cc02b-129">Значение</span><span class="sxs-lookup"><span data-stu-id="cc02b-129">Value.</span></span> <span data-ttu-id="cc02b-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="cc02b-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc02b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="cc02b-131">Relationships</span></span>
<span data-ttu-id="cc02b-132">Нет</span><span class="sxs-lookup"><span data-stu-id="cc02b-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc02b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc02b-133">JSON Representation</span></span>
<span data-ttu-id="cc02b-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc02b-134">Here is a JSON representation of the resource.</span></span>
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



