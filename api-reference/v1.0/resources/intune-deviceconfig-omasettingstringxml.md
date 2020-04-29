---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7218784b03489419fc3dbcf9aeb2aed4e4e78ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472967"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="ccf33-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="ccf33-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="ccf33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccf33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccf33-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccf33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccf33-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="ccf33-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="ccf33-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ccf33-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ccf33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccf33-108">Properties</span></span>
|<span data-ttu-id="ccf33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccf33-109">Property</span></span>|<span data-ttu-id="ccf33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ccf33-110">Type</span></span>|<span data-ttu-id="ccf33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ccf33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf33-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ccf33-112">displayName</span></span>|<span data-ttu-id="ccf33-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ccf33-113">String</span></span>|<span data-ttu-id="ccf33-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ccf33-114">Display Name.</span></span> <span data-ttu-id="ccf33-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ccf33-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ccf33-116">description</span><span class="sxs-lookup"><span data-stu-id="ccf33-116">description</span></span>|<span data-ttu-id="ccf33-117">String</span><span class="sxs-lookup"><span data-stu-id="ccf33-117">String</span></span>|<span data-ttu-id="ccf33-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="ccf33-118">Description.</span></span> <span data-ttu-id="ccf33-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ccf33-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ccf33-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="ccf33-120">omaUri</span></span>|<span data-ttu-id="ccf33-121">Строка</span><span class="sxs-lookup"><span data-stu-id="ccf33-121">String</span></span>|<span data-ttu-id="ccf33-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="ccf33-122">OMA.</span></span> <span data-ttu-id="ccf33-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ccf33-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ccf33-124">fileName</span><span class="sxs-lookup"><span data-stu-id="ccf33-124">fileName</span></span>|<span data-ttu-id="ccf33-125">String</span><span class="sxs-lookup"><span data-stu-id="ccf33-125">String</span></span>|<span data-ttu-id="ccf33-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="ccf33-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="ccf33-127">value</span><span class="sxs-lookup"><span data-stu-id="ccf33-127">value</span></span>|<span data-ttu-id="ccf33-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="ccf33-128">Binary</span></span>|<span data-ttu-id="ccf33-129">Значение</span><span class="sxs-lookup"><span data-stu-id="ccf33-129">Value.</span></span> <span data-ttu-id="ccf33-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="ccf33-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf33-131">Связи</span><span class="sxs-lookup"><span data-stu-id="ccf33-131">Relationships</span></span>
<span data-ttu-id="ccf33-132">Нет</span><span class="sxs-lookup"><span data-stu-id="ccf33-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccf33-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccf33-133">JSON Representation</span></span>
<span data-ttu-id="ccf33-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccf33-134">Here is a JSON representation of the resource.</span></span>
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







