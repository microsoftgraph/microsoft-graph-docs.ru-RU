---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99fa5ccf0b26ebd04ce232eb8bf4df9a9d4ace81
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755884"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="20d98-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="20d98-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="20d98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20d98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20d98-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20d98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20d98-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="20d98-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="20d98-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="20d98-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="20d98-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="20d98-108">Properties</span></span>
|<span data-ttu-id="20d98-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="20d98-109">Property</span></span>|<span data-ttu-id="20d98-110">Тип</span><span class="sxs-lookup"><span data-stu-id="20d98-110">Type</span></span>|<span data-ttu-id="20d98-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20d98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20d98-112">displayName</span><span class="sxs-lookup"><span data-stu-id="20d98-112">displayName</span></span>|<span data-ttu-id="20d98-113">String</span><span class="sxs-lookup"><span data-stu-id="20d98-113">String</span></span>|<span data-ttu-id="20d98-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="20d98-114">Display Name.</span></span> <span data-ttu-id="20d98-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="20d98-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="20d98-116">description</span><span class="sxs-lookup"><span data-stu-id="20d98-116">description</span></span>|<span data-ttu-id="20d98-117">String</span><span class="sxs-lookup"><span data-stu-id="20d98-117">String</span></span>|<span data-ttu-id="20d98-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="20d98-118">Description.</span></span> <span data-ttu-id="20d98-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="20d98-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="20d98-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="20d98-120">omaUri</span></span>|<span data-ttu-id="20d98-121">String</span><span class="sxs-lookup"><span data-stu-id="20d98-121">String</span></span>|<span data-ttu-id="20d98-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="20d98-122">OMA.</span></span> <span data-ttu-id="20d98-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="20d98-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="20d98-124">value</span><span class="sxs-lookup"><span data-stu-id="20d98-124">value</span></span>|<span data-ttu-id="20d98-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20d98-125">DateTimeOffset</span></span>|<span data-ttu-id="20d98-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="20d98-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20d98-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="20d98-127">Relationships</span></span>
<span data-ttu-id="20d98-128">Нет</span><span class="sxs-lookup"><span data-stu-id="20d98-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20d98-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20d98-129">JSON Representation</span></span>
<span data-ttu-id="20d98-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20d98-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```




