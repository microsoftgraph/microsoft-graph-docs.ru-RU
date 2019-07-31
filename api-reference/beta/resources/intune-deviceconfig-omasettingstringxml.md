---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: efc9a2ddd996088f88b85be55c9c7d6bfe62b86a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000790"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="84053-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="84053-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="84053-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84053-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84053-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84053-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84053-106">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="84053-106">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="84053-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="84053-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84053-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="84053-108">Properties</span></span>
|<span data-ttu-id="84053-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="84053-109">Property</span></span>|<span data-ttu-id="84053-110">Тип</span><span class="sxs-lookup"><span data-stu-id="84053-110">Type</span></span>|<span data-ttu-id="84053-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84053-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84053-112">displayName</span><span class="sxs-lookup"><span data-stu-id="84053-112">displayName</span></span>|<span data-ttu-id="84053-113">Строка</span><span class="sxs-lookup"><span data-stu-id="84053-113">String</span></span>|<span data-ttu-id="84053-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="84053-114">Display Name.</span></span> <span data-ttu-id="84053-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="84053-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="84053-116">description</span><span class="sxs-lookup"><span data-stu-id="84053-116">description</span></span>|<span data-ttu-id="84053-117">String</span><span class="sxs-lookup"><span data-stu-id="84053-117">String</span></span>|<span data-ttu-id="84053-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="84053-118">Description.</span></span> <span data-ttu-id="84053-119">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="84053-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="84053-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="84053-120">omaUri</span></span>|<span data-ttu-id="84053-121">Строка</span><span class="sxs-lookup"><span data-stu-id="84053-121">String</span></span>|<span data-ttu-id="84053-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="84053-122">OMA.</span></span> <span data-ttu-id="84053-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="84053-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="84053-124">fileName</span><span class="sxs-lookup"><span data-stu-id="84053-124">fileName</span></span>|<span data-ttu-id="84053-125">String</span><span class="sxs-lookup"><span data-stu-id="84053-125">String</span></span>|<span data-ttu-id="84053-126">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="84053-126">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="84053-127">value</span><span class="sxs-lookup"><span data-stu-id="84053-127">value</span></span>|<span data-ttu-id="84053-128">Двоичный</span><span class="sxs-lookup"><span data-stu-id="84053-128">Binary</span></span>|<span data-ttu-id="84053-129">Значение</span><span class="sxs-lookup"><span data-stu-id="84053-129">Value.</span></span> <span data-ttu-id="84053-130">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="84053-130">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="84053-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="84053-131">Relationships</span></span>
<span data-ttu-id="84053-132">Нет</span><span class="sxs-lookup"><span data-stu-id="84053-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84053-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84053-133">JSON Representation</span></span>
<span data-ttu-id="84053-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84053-134">Here is a JSON representation of the resource.</span></span>
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





