---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6713977ef36edc43f1d2e00cf489f9906e6bd929
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755856"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="25ad9-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="25ad9-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="25ad9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25ad9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25ad9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25ad9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25ad9-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="25ad9-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="25ad9-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25ad9-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25ad9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="25ad9-108">Properties</span></span>
|<span data-ttu-id="25ad9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="25ad9-109">Property</span></span>|<span data-ttu-id="25ad9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="25ad9-110">Type</span></span>|<span data-ttu-id="25ad9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="25ad9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25ad9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="25ad9-112">displayName</span></span>|<span data-ttu-id="25ad9-113">String</span><span class="sxs-lookup"><span data-stu-id="25ad9-113">String</span></span>|<span data-ttu-id="25ad9-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="25ad9-114">Display Name.</span></span> <span data-ttu-id="25ad9-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25ad9-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="25ad9-116">description</span><span class="sxs-lookup"><span data-stu-id="25ad9-116">description</span></span>|<span data-ttu-id="25ad9-117">String</span><span class="sxs-lookup"><span data-stu-id="25ad9-117">String</span></span>|<span data-ttu-id="25ad9-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="25ad9-118">Description.</span></span> <span data-ttu-id="25ad9-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25ad9-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="25ad9-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="25ad9-120">omaUri</span></span>|<span data-ttu-id="25ad9-121">String</span><span class="sxs-lookup"><span data-stu-id="25ad9-121">String</span></span>|<span data-ttu-id="25ad9-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="25ad9-122">OMA.</span></span> <span data-ttu-id="25ad9-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25ad9-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="25ad9-124">fileName</span><span class="sxs-lookup"><span data-stu-id="25ad9-124">fileName</span></span>|<span data-ttu-id="25ad9-125">String</span><span class="sxs-lookup"><span data-stu-id="25ad9-125">String</span></span>|<span data-ttu-id="25ad9-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="25ad9-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="25ad9-127">value</span><span class="sxs-lookup"><span data-stu-id="25ad9-127">value</span></span>|<span data-ttu-id="25ad9-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="25ad9-128">Binary</span></span>|<span data-ttu-id="25ad9-129">Значение</span><span class="sxs-lookup"><span data-stu-id="25ad9-129">Value.</span></span> <span data-ttu-id="25ad9-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="25ad9-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="25ad9-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="25ad9-131">Relationships</span></span>
<span data-ttu-id="25ad9-132">Нет</span><span class="sxs-lookup"><span data-stu-id="25ad9-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25ad9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25ad9-133">JSON Representation</span></span>
<span data-ttu-id="25ad9-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25ad9-134">Here is a JSON representation of the resource.</span></span>
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




