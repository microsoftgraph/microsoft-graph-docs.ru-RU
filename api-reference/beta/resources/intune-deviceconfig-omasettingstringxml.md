---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 976c95ed9ffa6674ddc185bb1723c7d7f9d054f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894021"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="b59d4-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="b59d4-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="b59d4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b59d4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b59d4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b59d4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b59d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b59d4-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="b59d4-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="b59d4-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b59d4-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b59d4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b59d4-109">Properties</span></span>
|<span data-ttu-id="b59d4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b59d4-110">Property</span></span>|<span data-ttu-id="b59d4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b59d4-111">Type</span></span>|<span data-ttu-id="b59d4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b59d4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b59d4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b59d4-113">displayName</span></span>|<span data-ttu-id="b59d4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b59d4-114">String</span></span>|<span data-ttu-id="b59d4-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b59d4-115">Display Name.</span></span> <span data-ttu-id="b59d4-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b59d4-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b59d4-117">описание</span><span class="sxs-lookup"><span data-stu-id="b59d4-117">description</span></span>|<span data-ttu-id="b59d4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="b59d4-118">String</span></span>|<span data-ttu-id="b59d4-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="b59d4-119">Description.</span></span> <span data-ttu-id="b59d4-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b59d4-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b59d4-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b59d4-121">omaUri</span></span>|<span data-ttu-id="b59d4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="b59d4-122">String</span></span>|<span data-ttu-id="b59d4-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="b59d4-123">OMA.</span></span> <span data-ttu-id="b59d4-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b59d4-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b59d4-125">fileName</span><span class="sxs-lookup"><span data-stu-id="b59d4-125">fileName</span></span>|<span data-ttu-id="b59d4-126">String</span><span class="sxs-lookup"><span data-stu-id="b59d4-126">String</span></span>|<span data-ttu-id="b59d4-127">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="b59d4-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="b59d4-128">value</span><span class="sxs-lookup"><span data-stu-id="b59d4-128">value</span></span>|<span data-ttu-id="b59d4-129">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b59d4-129">Binary</span></span>|<span data-ttu-id="b59d4-130">Значение</span><span class="sxs-lookup"><span data-stu-id="b59d4-130">Value.</span></span> <span data-ttu-id="b59d4-131">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="b59d4-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b59d4-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b59d4-132">Relationships</span></span>
<span data-ttu-id="b59d4-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b59d4-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b59d4-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b59d4-134">JSON Representation</span></span>
<span data-ttu-id="b59d4-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b59d4-135">Here is a JSON representation of the resource.</span></span>
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





