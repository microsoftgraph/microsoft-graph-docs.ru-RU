---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97ac2092573639db5d46386fe9475df26b136e80
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368501"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="21473-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="21473-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="21473-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21473-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21473-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="21473-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="21473-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21473-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21473-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21473-108">Properties</span></span>
|<span data-ttu-id="21473-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21473-109">Property</span></span>|<span data-ttu-id="21473-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21473-110">Type</span></span>|<span data-ttu-id="21473-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21473-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21473-112">displayName</span><span class="sxs-lookup"><span data-stu-id="21473-112">displayName</span></span>|<span data-ttu-id="21473-113">Строка</span><span class="sxs-lookup"><span data-stu-id="21473-113">String</span></span>|<span data-ttu-id="21473-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="21473-114">Display Name.</span></span> <span data-ttu-id="21473-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21473-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21473-116">description</span><span class="sxs-lookup"><span data-stu-id="21473-116">description</span></span>|<span data-ttu-id="21473-117">String</span><span class="sxs-lookup"><span data-stu-id="21473-117">String</span></span>|<span data-ttu-id="21473-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="21473-118">Description.</span></span> <span data-ttu-id="21473-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21473-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21473-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="21473-120">omaUri</span></span>|<span data-ttu-id="21473-121">String</span><span class="sxs-lookup"><span data-stu-id="21473-121">String</span></span>|<span data-ttu-id="21473-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="21473-122">OMA.</span></span> <span data-ttu-id="21473-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21473-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="21473-124">value</span><span class="sxs-lookup"><span data-stu-id="21473-124">value</span></span>|<span data-ttu-id="21473-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21473-125">DateTimeOffset</span></span>|<span data-ttu-id="21473-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="21473-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21473-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="21473-127">Relationships</span></span>
<span data-ttu-id="21473-128">Нет</span><span class="sxs-lookup"><span data-stu-id="21473-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21473-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21473-129">JSON Representation</span></span>
<span data-ttu-id="21473-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21473-130">Here is a JSON representation of the resource.</span></span>
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



