---
title: Тип ресурса omaSettingStringXml
description: Определение строки параметра OMA в формате XML.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7a2c25690f3084f79d6e80975c92aed9db0f1657
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989250"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="f40ad-103">Тип ресурса omaSettingStringXml</span><span class="sxs-lookup"><span data-stu-id="f40ad-103">omaSettingStringXml resource type</span></span>

<span data-ttu-id="f40ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f40ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f40ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f40ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f40ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f40ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f40ad-107">Определение строки параметра OMA в формате XML.</span><span class="sxs-lookup"><span data-stu-id="f40ad-107">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="f40ad-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f40ad-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f40ad-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f40ad-109">Properties</span></span>
|<span data-ttu-id="f40ad-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f40ad-110">Property</span></span>|<span data-ttu-id="f40ad-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f40ad-111">Type</span></span>|<span data-ttu-id="f40ad-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f40ad-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f40ad-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f40ad-113">displayName</span></span>|<span data-ttu-id="f40ad-114">String</span><span class="sxs-lookup"><span data-stu-id="f40ad-114">String</span></span>|<span data-ttu-id="f40ad-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f40ad-115">Display Name.</span></span> <span data-ttu-id="f40ad-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f40ad-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f40ad-117">description</span><span class="sxs-lookup"><span data-stu-id="f40ad-117">description</span></span>|<span data-ttu-id="f40ad-118">String</span><span class="sxs-lookup"><span data-stu-id="f40ad-118">String</span></span>|<span data-ttu-id="f40ad-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="f40ad-119">Description.</span></span> <span data-ttu-id="f40ad-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f40ad-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f40ad-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f40ad-121">omaUri</span></span>|<span data-ttu-id="f40ad-122">String</span><span class="sxs-lookup"><span data-stu-id="f40ad-122">String</span></span>|<span data-ttu-id="f40ad-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="f40ad-123">OMA.</span></span> <span data-ttu-id="f40ad-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f40ad-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f40ad-125">fileName</span><span class="sxs-lookup"><span data-stu-id="f40ad-125">fileName</span></span>|<span data-ttu-id="f40ad-126">String</span><span class="sxs-lookup"><span data-stu-id="f40ad-126">String</span></span>|<span data-ttu-id="f40ad-127">Имя файла, связанное со свойством Value (XML).</span><span class="sxs-lookup"><span data-stu-id="f40ad-127">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="f40ad-128">value</span><span class="sxs-lookup"><span data-stu-id="f40ad-128">value</span></span>|<span data-ttu-id="f40ad-129">Двоичный</span><span class="sxs-lookup"><span data-stu-id="f40ad-129">Binary</span></span>|<span data-ttu-id="f40ad-130">Значение</span><span class="sxs-lookup"><span data-stu-id="f40ad-130">Value.</span></span> <span data-ttu-id="f40ad-131">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="f40ad-131">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f40ad-132">Связи</span><span class="sxs-lookup"><span data-stu-id="f40ad-132">Relationships</span></span>
<span data-ttu-id="f40ad-133">Нет</span><span class="sxs-lookup"><span data-stu-id="f40ad-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f40ad-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f40ad-134">JSON Representation</span></span>
<span data-ttu-id="f40ad-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f40ad-135">Here is a JSON representation of the resource.</span></span>
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






