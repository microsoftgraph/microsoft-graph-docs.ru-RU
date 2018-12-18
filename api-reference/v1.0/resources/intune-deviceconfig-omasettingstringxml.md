---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
ms.openlocfilehash: c7f7d07a94550d86e6507e9202195d09e9555f60
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332013"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="8f473-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="8f473-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="8f473-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f473-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f473-105">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="8f473-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="8f473-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f473-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f473-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f473-107">Properties</span></span>
|<span data-ttu-id="8f473-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f473-108">Property</span></span>|<span data-ttu-id="8f473-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8f473-109">Type</span></span>|<span data-ttu-id="8f473-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f473-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f473-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8f473-111">displayName</span></span>|<span data-ttu-id="8f473-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8f473-112">String</span></span>|<span data-ttu-id="8f473-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="8f473-113">Display Name.</span></span> <span data-ttu-id="8f473-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f473-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f473-115">описание</span><span class="sxs-lookup"><span data-stu-id="8f473-115">description</span></span>|<span data-ttu-id="8f473-116">Строка</span><span class="sxs-lookup"><span data-stu-id="8f473-116">String</span></span>|<span data-ttu-id="8f473-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="8f473-117">Description.</span></span> <span data-ttu-id="8f473-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f473-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f473-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8f473-119">omaUri</span></span>|<span data-ttu-id="8f473-120">Строка</span><span class="sxs-lookup"><span data-stu-id="8f473-120">String</span></span>|<span data-ttu-id="8f473-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8f473-121">OMA.</span></span> <span data-ttu-id="8f473-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8f473-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8f473-123">fileName</span><span class="sxs-lookup"><span data-stu-id="8f473-123">fileName</span></span>|<span data-ttu-id="8f473-124">String</span><span class="sxs-lookup"><span data-stu-id="8f473-124">String</span></span>|<span data-ttu-id="8f473-125">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="8f473-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="8f473-126">value</span><span class="sxs-lookup"><span data-stu-id="8f473-126">value</span></span>|<span data-ttu-id="8f473-127">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8f473-127">Binary</span></span>|<span data-ttu-id="8f473-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8f473-128">Value.</span></span> <span data-ttu-id="8f473-129">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="8f473-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f473-130">Связи</span><span class="sxs-lookup"><span data-stu-id="8f473-130">Relationships</span></span>
<span data-ttu-id="8f473-131">Нет</span><span class="sxs-lookup"><span data-stu-id="8f473-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f473-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f473-132">JSON Representation</span></span>
<span data-ttu-id="8f473-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f473-133">Here is a JSON representation of the resource.</span></span>
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



