---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
ms.openlocfilehash: ecdc22f698479ba25a2cce4ce822cda633c582ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024530"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="8dd0e-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="8dd0e-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="8dd0e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8dd0e-105">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-105">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="8dd0e-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8dd0e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8dd0e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8dd0e-107">Properties</span></span>
|<span data-ttu-id="8dd0e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd0e-108">Property</span></span>|<span data-ttu-id="8dd0e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd0e-109">Type</span></span>|<span data-ttu-id="8dd0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dd0e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8dd0e-111">displayName</span></span>|<span data-ttu-id="8dd0e-112">String</span><span class="sxs-lookup"><span data-stu-id="8dd0e-112">String</span></span>|<span data-ttu-id="8dd0e-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-113">Display Name.</span></span> <span data-ttu-id="8dd0e-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8dd0e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8dd0e-115">описание</span><span class="sxs-lookup"><span data-stu-id="8dd0e-115">description</span></span>|<span data-ttu-id="8dd0e-116">String</span><span class="sxs-lookup"><span data-stu-id="8dd0e-116">String</span></span>|<span data-ttu-id="8dd0e-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-117">Description.</span></span> <span data-ttu-id="8dd0e-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8dd0e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8dd0e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8dd0e-119">omaUri</span></span>|<span data-ttu-id="8dd0e-120">String</span><span class="sxs-lookup"><span data-stu-id="8dd0e-120">String</span></span>|<span data-ttu-id="8dd0e-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-121">OMA.</span></span> <span data-ttu-id="8dd0e-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8dd0e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8dd0e-123">fileName</span><span class="sxs-lookup"><span data-stu-id="8dd0e-123">fileName</span></span>|<span data-ttu-id="8dd0e-124">String</span><span class="sxs-lookup"><span data-stu-id="8dd0e-124">String</span></span>|<span data-ttu-id="8dd0e-125">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="8dd0e-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="8dd0e-126">value</span><span class="sxs-lookup"><span data-stu-id="8dd0e-126">value</span></span>|<span data-ttu-id="8dd0e-127">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8dd0e-127">Binary</span></span>|<span data-ttu-id="8dd0e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8dd0e-128">Value.</span></span> <span data-ttu-id="8dd0e-129">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="8dd0e-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dd0e-130">Связи</span><span class="sxs-lookup"><span data-stu-id="8dd0e-130">Relationships</span></span>
<span data-ttu-id="8dd0e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="8dd0e-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8dd0e-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8dd0e-132">JSON Representation</span></span>
<span data-ttu-id="8dd0e-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dd0e-133">Here is a JSON representation of the resource.</span></span>
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



