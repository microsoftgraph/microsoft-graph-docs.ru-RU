---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0fa631992288695b069a6317128fa369ed42b4d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967432"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="57044-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="57044-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="57044-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57044-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57044-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57044-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57044-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="57044-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57044-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="57044-107">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="57044-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="57044-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57044-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="57044-109">Properties</span></span>
|<span data-ttu-id="57044-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="57044-110">Property</span></span>|<span data-ttu-id="57044-111">Тип</span><span class="sxs-lookup"><span data-stu-id="57044-111">Type</span></span>|<span data-ttu-id="57044-112">Описание</span><span class="sxs-lookup"><span data-stu-id="57044-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57044-113">displayName</span><span class="sxs-lookup"><span data-stu-id="57044-113">displayName</span></span>|<span data-ttu-id="57044-114">Строка</span><span class="sxs-lookup"><span data-stu-id="57044-114">String</span></span>|<span data-ttu-id="57044-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="57044-115">Display Name.</span></span> <span data-ttu-id="57044-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="57044-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="57044-117">описание</span><span class="sxs-lookup"><span data-stu-id="57044-117">description</span></span>|<span data-ttu-id="57044-118">Строка</span><span class="sxs-lookup"><span data-stu-id="57044-118">String</span></span>|<span data-ttu-id="57044-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="57044-119">Description.</span></span> <span data-ttu-id="57044-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="57044-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="57044-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="57044-121">omaUri</span></span>|<span data-ttu-id="57044-122">Строка</span><span class="sxs-lookup"><span data-stu-id="57044-122">String</span></span>|<span data-ttu-id="57044-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="57044-123">OMA.</span></span> <span data-ttu-id="57044-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="57044-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="57044-125">fileName</span><span class="sxs-lookup"><span data-stu-id="57044-125">fileName</span></span>|<span data-ttu-id="57044-126">String</span><span class="sxs-lookup"><span data-stu-id="57044-126">String</span></span>|<span data-ttu-id="57044-127">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="57044-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="57044-128">value</span><span class="sxs-lookup"><span data-stu-id="57044-128">value</span></span>|<span data-ttu-id="57044-129">Двоичный</span><span class="sxs-lookup"><span data-stu-id="57044-129">Binary</span></span>|<span data-ttu-id="57044-130">Значение</span><span class="sxs-lookup"><span data-stu-id="57044-130">Value.</span></span> <span data-ttu-id="57044-131">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="57044-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="57044-132">Связи</span><span class="sxs-lookup"><span data-stu-id="57044-132">Relationships</span></span>
<span data-ttu-id="57044-133">Нет</span><span class="sxs-lookup"><span data-stu-id="57044-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57044-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57044-134">JSON Representation</span></span>
<span data-ttu-id="57044-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57044-135">Here is a JSON representation of the resource.</span></span>
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





