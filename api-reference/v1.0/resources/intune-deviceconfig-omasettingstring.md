---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a647b532704af6892af7d65714d47ad16eb00eaf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755863"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="b634d-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="b634d-103">omaSettingString resource type</span></span>

<span data-ttu-id="b634d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b634d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b634d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b634d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b634d-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="b634d-106">OMA Settings String definition.</span></span>


<span data-ttu-id="b634d-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b634d-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b634d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b634d-108">Properties</span></span>
|<span data-ttu-id="b634d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b634d-109">Property</span></span>|<span data-ttu-id="b634d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b634d-110">Type</span></span>|<span data-ttu-id="b634d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b634d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b634d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b634d-112">displayName</span></span>|<span data-ttu-id="b634d-113">String</span><span class="sxs-lookup"><span data-stu-id="b634d-113">String</span></span>|<span data-ttu-id="b634d-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b634d-114">Display Name.</span></span> <span data-ttu-id="b634d-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b634d-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b634d-116">description</span><span class="sxs-lookup"><span data-stu-id="b634d-116">description</span></span>|<span data-ttu-id="b634d-117">String</span><span class="sxs-lookup"><span data-stu-id="b634d-117">String</span></span>|<span data-ttu-id="b634d-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="b634d-118">Description.</span></span> <span data-ttu-id="b634d-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b634d-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b634d-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="b634d-120">omaUri</span></span>|<span data-ttu-id="b634d-121">String</span><span class="sxs-lookup"><span data-stu-id="b634d-121">String</span></span>|<span data-ttu-id="b634d-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="b634d-122">OMA.</span></span> <span data-ttu-id="b634d-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b634d-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b634d-124">value</span><span class="sxs-lookup"><span data-stu-id="b634d-124">value</span></span>|<span data-ttu-id="b634d-125">String</span><span class="sxs-lookup"><span data-stu-id="b634d-125">String</span></span>|<span data-ttu-id="b634d-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b634d-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b634d-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="b634d-127">Relationships</span></span>
<span data-ttu-id="b634d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b634d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b634d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b634d-129">JSON Representation</span></span>
<span data-ttu-id="b634d-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b634d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```




