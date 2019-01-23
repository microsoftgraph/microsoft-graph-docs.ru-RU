---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e47ba7fce929e114282c6aa88605d9f185618
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419438"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="3e51c-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="3e51c-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="3e51c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e51c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e51c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e51c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e51c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e51c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e51c-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="3e51c-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="3e51c-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e51c-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e51c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e51c-109">Properties</span></span>
|<span data-ttu-id="3e51c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e51c-110">Property</span></span>|<span data-ttu-id="3e51c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3e51c-111">Type</span></span>|<span data-ttu-id="3e51c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3e51c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e51c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="3e51c-113">displayName</span></span>|<span data-ttu-id="3e51c-114">String</span><span class="sxs-lookup"><span data-stu-id="3e51c-114">String</span></span>|<span data-ttu-id="3e51c-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3e51c-115">Display Name.</span></span> <span data-ttu-id="3e51c-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e51c-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e51c-117">description</span><span class="sxs-lookup"><span data-stu-id="3e51c-117">description</span></span>|<span data-ttu-id="3e51c-118">String</span><span class="sxs-lookup"><span data-stu-id="3e51c-118">String</span></span>|<span data-ttu-id="3e51c-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="3e51c-119">Description.</span></span> <span data-ttu-id="3e51c-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e51c-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e51c-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="3e51c-121">omaUri</span></span>|<span data-ttu-id="3e51c-122">String</span><span class="sxs-lookup"><span data-stu-id="3e51c-122">String</span></span>|<span data-ttu-id="3e51c-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="3e51c-123">OMA.</span></span> <span data-ttu-id="3e51c-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e51c-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3e51c-125">fileName</span><span class="sxs-lookup"><span data-stu-id="3e51c-125">fileName</span></span>|<span data-ttu-id="3e51c-126">String</span><span class="sxs-lookup"><span data-stu-id="3e51c-126">String</span></span>|<span data-ttu-id="3e51c-127">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="3e51c-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="3e51c-128">value</span><span class="sxs-lookup"><span data-stu-id="3e51c-128">value</span></span>|<span data-ttu-id="3e51c-129">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3e51c-129">Binary</span></span>|<span data-ttu-id="3e51c-130">Значение</span><span class="sxs-lookup"><span data-stu-id="3e51c-130">Value.</span></span> <span data-ttu-id="3e51c-131">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="3e51c-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e51c-132">Связи</span><span class="sxs-lookup"><span data-stu-id="3e51c-132">Relationships</span></span>
<span data-ttu-id="3e51c-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3e51c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e51c-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e51c-134">JSON Representation</span></span>
<span data-ttu-id="3e51c-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e51c-135">Here is a JSON representation of the resource.</span></span>
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




