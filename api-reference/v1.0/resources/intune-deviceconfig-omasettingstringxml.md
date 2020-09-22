---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c85dbc033264715026227be4055a0bf3130a5cc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988263"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="473d0-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="473d0-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="473d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="473d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="473d0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="473d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="473d0-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="473d0-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="473d0-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="473d0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="473d0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="473d0-108">Properties</span></span>
|<span data-ttu-id="473d0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="473d0-109">Property</span></span>|<span data-ttu-id="473d0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="473d0-110">Type</span></span>|<span data-ttu-id="473d0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="473d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="473d0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="473d0-112">displayName</span></span>|<span data-ttu-id="473d0-113">String</span><span class="sxs-lookup"><span data-stu-id="473d0-113">String</span></span>|<span data-ttu-id="473d0-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="473d0-114">Display Name.</span></span> <span data-ttu-id="473d0-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="473d0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="473d0-116">description</span><span class="sxs-lookup"><span data-stu-id="473d0-116">description</span></span>|<span data-ttu-id="473d0-117">String</span><span class="sxs-lookup"><span data-stu-id="473d0-117">String</span></span>|<span data-ttu-id="473d0-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="473d0-118">Description.</span></span> <span data-ttu-id="473d0-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="473d0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="473d0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="473d0-120">omaUri</span></span>|<span data-ttu-id="473d0-121">String</span><span class="sxs-lookup"><span data-stu-id="473d0-121">String</span></span>|<span data-ttu-id="473d0-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="473d0-122">OMA.</span></span> <span data-ttu-id="473d0-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="473d0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="473d0-124">fileName</span><span class="sxs-lookup"><span data-stu-id="473d0-124">fileName</span></span>|<span data-ttu-id="473d0-125">String</span><span class="sxs-lookup"><span data-stu-id="473d0-125">String</span></span>|<span data-ttu-id="473d0-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="473d0-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="473d0-127">value</span><span class="sxs-lookup"><span data-stu-id="473d0-127">value</span></span>|<span data-ttu-id="473d0-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="473d0-128">Binary</span></span>|<span data-ttu-id="473d0-129">Значение</span><span class="sxs-lookup"><span data-stu-id="473d0-129">Value.</span></span> <span data-ttu-id="473d0-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="473d0-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="473d0-131">Связи</span><span class="sxs-lookup"><span data-stu-id="473d0-131">Relationships</span></span>
<span data-ttu-id="473d0-132">Нет</span><span class="sxs-lookup"><span data-stu-id="473d0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="473d0-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="473d0-133">JSON Representation</span></span>
<span data-ttu-id="473d0-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="473d0-134">Here is a JSON representation of the resource.</span></span>
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









