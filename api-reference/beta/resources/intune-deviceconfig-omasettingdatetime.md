---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 283b41018ad89b157c679c8b532c869d350b9182
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144466"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="38793-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="38793-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="38793-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38793-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38793-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38793-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38793-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="38793-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="38793-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38793-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38793-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38793-108">Properties</span></span>
|<span data-ttu-id="38793-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38793-109">Property</span></span>|<span data-ttu-id="38793-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38793-110">Type</span></span>|<span data-ttu-id="38793-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38793-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38793-112">displayName</span><span class="sxs-lookup"><span data-stu-id="38793-112">displayName</span></span>|<span data-ttu-id="38793-113">String</span><span class="sxs-lookup"><span data-stu-id="38793-113">String</span></span>|<span data-ttu-id="38793-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="38793-114">Display Name.</span></span> <span data-ttu-id="38793-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38793-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38793-116">description</span><span class="sxs-lookup"><span data-stu-id="38793-116">description</span></span>|<span data-ttu-id="38793-117">String</span><span class="sxs-lookup"><span data-stu-id="38793-117">String</span></span>|<span data-ttu-id="38793-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="38793-118">Description.</span></span> <span data-ttu-id="38793-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38793-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38793-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="38793-120">omaUri</span></span>|<span data-ttu-id="38793-121">String</span><span class="sxs-lookup"><span data-stu-id="38793-121">String</span></span>|<span data-ttu-id="38793-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="38793-122">OMA.</span></span> <span data-ttu-id="38793-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38793-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38793-124">value</span><span class="sxs-lookup"><span data-stu-id="38793-124">value</span></span>|<span data-ttu-id="38793-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38793-125">DateTimeOffset</span></span>|<span data-ttu-id="38793-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="38793-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38793-127">Связи</span><span class="sxs-lookup"><span data-stu-id="38793-127">Relationships</span></span>
<span data-ttu-id="38793-128">Нет</span><span class="sxs-lookup"><span data-stu-id="38793-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38793-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38793-129">JSON Representation</span></span>
<span data-ttu-id="38793-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38793-130">Here is a JSON representation of the resource.</span></span>
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




