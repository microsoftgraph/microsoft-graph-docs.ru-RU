---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 797588826496201715295dbc48a9e5e8c5d4f523
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532422"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="2de9e-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="2de9e-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="2de9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2de9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2de9e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2de9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2de9e-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="2de9e-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="2de9e-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2de9e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2de9e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2de9e-108">Properties</span></span>
|<span data-ttu-id="2de9e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2de9e-109">Property</span></span>|<span data-ttu-id="2de9e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2de9e-110">Type</span></span>|<span data-ttu-id="2de9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2de9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2de9e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2de9e-112">displayName</span></span>|<span data-ttu-id="2de9e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2de9e-113">String</span></span>|<span data-ttu-id="2de9e-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2de9e-114">Display Name.</span></span> <span data-ttu-id="2de9e-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2de9e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2de9e-116">description</span><span class="sxs-lookup"><span data-stu-id="2de9e-116">description</span></span>|<span data-ttu-id="2de9e-117">String</span><span class="sxs-lookup"><span data-stu-id="2de9e-117">String</span></span>|<span data-ttu-id="2de9e-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="2de9e-118">Description.</span></span> <span data-ttu-id="2de9e-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2de9e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2de9e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="2de9e-120">omaUri</span></span>|<span data-ttu-id="2de9e-121">Строка</span><span class="sxs-lookup"><span data-stu-id="2de9e-121">String</span></span>|<span data-ttu-id="2de9e-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="2de9e-122">OMA.</span></span> <span data-ttu-id="2de9e-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2de9e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2de9e-124">fileName</span><span class="sxs-lookup"><span data-stu-id="2de9e-124">fileName</span></span>|<span data-ttu-id="2de9e-125">String</span><span class="sxs-lookup"><span data-stu-id="2de9e-125">String</span></span>|<span data-ttu-id="2de9e-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="2de9e-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="2de9e-127">value</span><span class="sxs-lookup"><span data-stu-id="2de9e-127">value</span></span>|<span data-ttu-id="2de9e-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="2de9e-128">Binary</span></span>|<span data-ttu-id="2de9e-129">Значение</span><span class="sxs-lookup"><span data-stu-id="2de9e-129">Value.</span></span> <span data-ttu-id="2de9e-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="2de9e-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2de9e-131">Связи</span><span class="sxs-lookup"><span data-stu-id="2de9e-131">Relationships</span></span>
<span data-ttu-id="2de9e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="2de9e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2de9e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2de9e-133">JSON Representation</span></span>
<span data-ttu-id="2de9e-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2de9e-134">Here is a JSON representation of the resource.</span></span>
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




