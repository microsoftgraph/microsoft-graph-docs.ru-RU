---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6291fc5b81de9dea1bfa67515f4df296d9e3001e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978155"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="bc082-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="bc082-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="bc082-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc082-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc082-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc082-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="bc082-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="bc082-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc082-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc082-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc082-108">Properties</span></span>
|<span data-ttu-id="bc082-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc082-109">Property</span></span>|<span data-ttu-id="bc082-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bc082-110">Type</span></span>|<span data-ttu-id="bc082-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bc082-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc082-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bc082-112">displayName</span></span>|<span data-ttu-id="bc082-113">String</span><span class="sxs-lookup"><span data-stu-id="bc082-113">String</span></span>|<span data-ttu-id="bc082-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bc082-114">Display Name.</span></span> <span data-ttu-id="bc082-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc082-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc082-116">description</span><span class="sxs-lookup"><span data-stu-id="bc082-116">description</span></span>|<span data-ttu-id="bc082-117">String</span><span class="sxs-lookup"><span data-stu-id="bc082-117">String</span></span>|<span data-ttu-id="bc082-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="bc082-118">Description.</span></span> <span data-ttu-id="bc082-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc082-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc082-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="bc082-120">omaUri</span></span>|<span data-ttu-id="bc082-121">String</span><span class="sxs-lookup"><span data-stu-id="bc082-121">String</span></span>|<span data-ttu-id="bc082-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="bc082-122">OMA.</span></span> <span data-ttu-id="bc082-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bc082-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc082-124">value</span><span class="sxs-lookup"><span data-stu-id="bc082-124">value</span></span>|<span data-ttu-id="bc082-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc082-125">DateTimeOffset</span></span>|<span data-ttu-id="bc082-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="bc082-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc082-127">Связи</span><span class="sxs-lookup"><span data-stu-id="bc082-127">Relationships</span></span>
<span data-ttu-id="bc082-128">Нет</span><span class="sxs-lookup"><span data-stu-id="bc082-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc082-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc082-129">JSON Representation</span></span>
<span data-ttu-id="bc082-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc082-130">Here is a JSON representation of the resource.</span></span>
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









