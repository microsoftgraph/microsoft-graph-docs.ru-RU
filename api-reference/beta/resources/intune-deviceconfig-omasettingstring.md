---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53840e360446975dcbe6fda170ea26892fce3983
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950951"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="1878b-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="1878b-103">omaSettingString resource type</span></span>

> <span data-ttu-id="1878b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1878b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1878b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1878b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1878b-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="1878b-106">OMA Settings String definition.</span></span>


<span data-ttu-id="1878b-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1878b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1878b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1878b-108">Properties</span></span>
|<span data-ttu-id="1878b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1878b-109">Property</span></span>|<span data-ttu-id="1878b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1878b-110">Type</span></span>|<span data-ttu-id="1878b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1878b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1878b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1878b-112">displayName</span></span>|<span data-ttu-id="1878b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1878b-113">String</span></span>|<span data-ttu-id="1878b-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1878b-114">Display Name.</span></span> <span data-ttu-id="1878b-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1878b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1878b-116">description</span><span class="sxs-lookup"><span data-stu-id="1878b-116">description</span></span>|<span data-ttu-id="1878b-117">String</span><span class="sxs-lookup"><span data-stu-id="1878b-117">String</span></span>|<span data-ttu-id="1878b-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="1878b-118">Description.</span></span> <span data-ttu-id="1878b-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1878b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1878b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="1878b-120">omaUri</span></span>|<span data-ttu-id="1878b-121">String</span><span class="sxs-lookup"><span data-stu-id="1878b-121">String</span></span>|<span data-ttu-id="1878b-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="1878b-122">OMA.</span></span> <span data-ttu-id="1878b-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1878b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1878b-124">value</span><span class="sxs-lookup"><span data-stu-id="1878b-124">value</span></span>|<span data-ttu-id="1878b-125">Строка</span><span class="sxs-lookup"><span data-stu-id="1878b-125">String</span></span>|<span data-ttu-id="1878b-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1878b-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1878b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1878b-127">Relationships</span></span>
<span data-ttu-id="1878b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1878b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1878b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1878b-129">JSON Representation</span></span>
<span data-ttu-id="1878b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1878b-130">Here is a JSON representation of the resource.</span></span>
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




