---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b33dde8c6d24432d1eb5b4823873a9da712faf7d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529552"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="c2246-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="c2246-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="c2246-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2246-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2246-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2246-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2246-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2246-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="c2246-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="c2246-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2246-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2246-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2246-109">Properties</span></span>
|<span data-ttu-id="c2246-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2246-110">Property</span></span>|<span data-ttu-id="c2246-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2246-111">Type</span></span>|<span data-ttu-id="c2246-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2246-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2246-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c2246-113">displayName</span></span>|<span data-ttu-id="c2246-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c2246-114">String</span></span>|<span data-ttu-id="c2246-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2246-115">Display Name.</span></span> <span data-ttu-id="c2246-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2246-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2246-117">description</span><span class="sxs-lookup"><span data-stu-id="c2246-117">description</span></span>|<span data-ttu-id="c2246-118">String</span><span class="sxs-lookup"><span data-stu-id="c2246-118">String</span></span>|<span data-ttu-id="c2246-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="c2246-119">Description.</span></span> <span data-ttu-id="c2246-120">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2246-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2246-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="c2246-121">omaUri</span></span>|<span data-ttu-id="c2246-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c2246-122">String</span></span>|<span data-ttu-id="c2246-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="c2246-123">OMA.</span></span> <span data-ttu-id="c2246-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2246-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2246-125">fileName</span><span class="sxs-lookup"><span data-stu-id="c2246-125">fileName</span></span>|<span data-ttu-id="c2246-126">String</span><span class="sxs-lookup"><span data-stu-id="c2246-126">String</span></span>|<span data-ttu-id="c2246-127">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="c2246-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="c2246-128">value</span><span class="sxs-lookup"><span data-stu-id="c2246-128">value</span></span>|<span data-ttu-id="c2246-129">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c2246-129">Binary</span></span>|<span data-ttu-id="c2246-130">Значение</span><span class="sxs-lookup"><span data-stu-id="c2246-130">Value.</span></span> <span data-ttu-id="c2246-131">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="c2246-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2246-132">Связи</span><span class="sxs-lookup"><span data-stu-id="c2246-132">Relationships</span></span>
<span data-ttu-id="c2246-133">Нет</span><span class="sxs-lookup"><span data-stu-id="c2246-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2246-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2246-134">JSON Representation</span></span>
<span data-ttu-id="c2246-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2246-135">Here is a JSON representation of the resource.</span></span>
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



