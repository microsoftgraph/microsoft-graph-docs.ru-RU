---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f95201a725969fa125cdf949874686b9155fc3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568796"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="8526b-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="8526b-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="8526b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8526b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8526b-105">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="8526b-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="8526b-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8526b-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8526b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8526b-107">Properties</span></span>
|<span data-ttu-id="8526b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8526b-108">Property</span></span>|<span data-ttu-id="8526b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8526b-109">Type</span></span>|<span data-ttu-id="8526b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8526b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8526b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8526b-111">displayName</span></span>|<span data-ttu-id="8526b-112">String</span><span class="sxs-lookup"><span data-stu-id="8526b-112">String</span></span>|<span data-ttu-id="8526b-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="8526b-113">Display Name.</span></span> <span data-ttu-id="8526b-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8526b-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8526b-115">description</span><span class="sxs-lookup"><span data-stu-id="8526b-115">description</span></span>|<span data-ttu-id="8526b-116">String</span><span class="sxs-lookup"><span data-stu-id="8526b-116">String</span></span>|<span data-ttu-id="8526b-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="8526b-117">Description.</span></span> <span data-ttu-id="8526b-118">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8526b-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8526b-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8526b-119">omaUri</span></span>|<span data-ttu-id="8526b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="8526b-120">String</span></span>|<span data-ttu-id="8526b-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="8526b-121">OMA.</span></span> <span data-ttu-id="8526b-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8526b-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8526b-123">fileName</span><span class="sxs-lookup"><span data-stu-id="8526b-123">fileName</span></span>|<span data-ttu-id="8526b-124">String</span><span class="sxs-lookup"><span data-stu-id="8526b-124">String</span></span>|<span data-ttu-id="8526b-125">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="8526b-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="8526b-126">value</span><span class="sxs-lookup"><span data-stu-id="8526b-126">value</span></span>|<span data-ttu-id="8526b-127">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8526b-127">Binary</span></span>|<span data-ttu-id="8526b-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8526b-128">Value.</span></span> <span data-ttu-id="8526b-129">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="8526b-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8526b-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="8526b-130">Relationships</span></span>
<span data-ttu-id="8526b-131">Нет</span><span class="sxs-lookup"><span data-stu-id="8526b-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8526b-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8526b-132">JSON Representation</span></span>
<span data-ttu-id="8526b-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8526b-133">Here is a JSON representation of the resource.</span></span>
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



