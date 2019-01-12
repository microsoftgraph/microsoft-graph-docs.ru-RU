---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e34dc1ebdfff2692d35d258492bc58cb26282198
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911485"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="d6cf9-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="d6cf9-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="d6cf9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6cf9-105">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="d6cf9-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6cf9-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6cf9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6cf9-107">Properties</span></span>
|<span data-ttu-id="d6cf9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6cf9-108">Property</span></span>|<span data-ttu-id="d6cf9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6cf9-109">Type</span></span>|<span data-ttu-id="d6cf9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6cf9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6cf9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d6cf9-111">displayName</span></span>|<span data-ttu-id="d6cf9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="d6cf9-112">String</span></span>|<span data-ttu-id="d6cf9-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-113">Display Name.</span></span> <span data-ttu-id="d6cf9-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6cf9-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6cf9-115">описание</span><span class="sxs-lookup"><span data-stu-id="d6cf9-115">description</span></span>|<span data-ttu-id="d6cf9-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d6cf9-116">String</span></span>|<span data-ttu-id="d6cf9-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-117">Description.</span></span> <span data-ttu-id="d6cf9-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6cf9-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6cf9-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d6cf9-119">omaUri</span></span>|<span data-ttu-id="d6cf9-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d6cf9-120">String</span></span>|<span data-ttu-id="d6cf9-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-121">OMA.</span></span> <span data-ttu-id="d6cf9-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d6cf9-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d6cf9-123">fileName</span><span class="sxs-lookup"><span data-stu-id="d6cf9-123">fileName</span></span>|<span data-ttu-id="d6cf9-124">String</span><span class="sxs-lookup"><span data-stu-id="d6cf9-124">String</span></span>|<span data-ttu-id="d6cf9-125">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="d6cf9-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="d6cf9-126">value</span><span class="sxs-lookup"><span data-stu-id="d6cf9-126">value</span></span>|<span data-ttu-id="d6cf9-127">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d6cf9-127">Binary</span></span>|<span data-ttu-id="d6cf9-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d6cf9-128">Value.</span></span> <span data-ttu-id="d6cf9-129">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="d6cf9-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6cf9-130">Связи</span><span class="sxs-lookup"><span data-stu-id="d6cf9-130">Relationships</span></span>
<span data-ttu-id="d6cf9-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d6cf9-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6cf9-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6cf9-132">JSON Representation</span></span>
<span data-ttu-id="d6cf9-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6cf9-133">Here is a JSON representation of the resource.</span></span>
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



