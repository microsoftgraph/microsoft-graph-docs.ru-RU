---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 077593048b6dc1aa2611b9e87c506db43fffe922
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359910"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="4b4e0-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="4b4e0-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="4b4e0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b4e0-105">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="4b4e0-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b4e0-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b4e0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b4e0-107">Properties</span></span>
|<span data-ttu-id="4b4e0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b4e0-108">Property</span></span>|<span data-ttu-id="4b4e0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b4e0-109">Type</span></span>|<span data-ttu-id="4b4e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b4e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b4e0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4b4e0-111">displayName</span></span>|<span data-ttu-id="4b4e0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4b4e0-112">String</span></span>|<span data-ttu-id="4b4e0-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-113">Display Name.</span></span> <span data-ttu-id="4b4e0-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b4e0-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b4e0-115">description</span><span class="sxs-lookup"><span data-stu-id="4b4e0-115">description</span></span>|<span data-ttu-id="4b4e0-116">String</span><span class="sxs-lookup"><span data-stu-id="4b4e0-116">String</span></span>|<span data-ttu-id="4b4e0-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-117">Description.</span></span> <span data-ttu-id="4b4e0-118">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b4e0-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b4e0-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4b4e0-119">omaUri</span></span>|<span data-ttu-id="4b4e0-120">Строка</span><span class="sxs-lookup"><span data-stu-id="4b4e0-120">String</span></span>|<span data-ttu-id="4b4e0-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-121">OMA.</span></span> <span data-ttu-id="4b4e0-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b4e0-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b4e0-123">fileName</span><span class="sxs-lookup"><span data-stu-id="4b4e0-123">fileName</span></span>|<span data-ttu-id="4b4e0-124">String</span><span class="sxs-lookup"><span data-stu-id="4b4e0-124">String</span></span>|<span data-ttu-id="4b4e0-125">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="4b4e0-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="4b4e0-126">value</span><span class="sxs-lookup"><span data-stu-id="4b4e0-126">value</span></span>|<span data-ttu-id="4b4e0-127">Двоичный</span><span class="sxs-lookup"><span data-stu-id="4b4e0-127">Binary</span></span>|<span data-ttu-id="4b4e0-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4b4e0-128">Value.</span></span> <span data-ttu-id="4b4e0-129">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="4b4e0-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b4e0-130">Связи</span><span class="sxs-lookup"><span data-stu-id="4b4e0-130">Relationships</span></span>
<span data-ttu-id="4b4e0-131">Нет</span><span class="sxs-lookup"><span data-stu-id="4b4e0-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b4e0-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b4e0-132">JSON Representation</span></span>
<span data-ttu-id="4b4e0-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b4e0-133">Here is a JSON representation of the resource.</span></span>
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




