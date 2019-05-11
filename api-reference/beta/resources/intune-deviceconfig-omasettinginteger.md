---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef33fd372d797822a334a4b218df44572648b166
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951077"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="d07ef-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="d07ef-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="d07ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d07ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d07ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d07ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d07ef-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d07ef-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="d07ef-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d07ef-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d07ef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d07ef-108">Properties</span></span>
|<span data-ttu-id="d07ef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d07ef-109">Property</span></span>|<span data-ttu-id="d07ef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d07ef-110">Type</span></span>|<span data-ttu-id="d07ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d07ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d07ef-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d07ef-112">displayName</span></span>|<span data-ttu-id="d07ef-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d07ef-113">String</span></span>|<span data-ttu-id="d07ef-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d07ef-114">Display Name.</span></span> <span data-ttu-id="d07ef-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d07ef-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d07ef-116">description</span><span class="sxs-lookup"><span data-stu-id="d07ef-116">description</span></span>|<span data-ttu-id="d07ef-117">String</span><span class="sxs-lookup"><span data-stu-id="d07ef-117">String</span></span>|<span data-ttu-id="d07ef-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="d07ef-118">Description.</span></span> <span data-ttu-id="d07ef-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d07ef-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d07ef-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d07ef-120">omaUri</span></span>|<span data-ttu-id="d07ef-121">String</span><span class="sxs-lookup"><span data-stu-id="d07ef-121">String</span></span>|<span data-ttu-id="d07ef-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d07ef-122">OMA.</span></span> <span data-ttu-id="d07ef-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d07ef-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d07ef-124">value</span><span class="sxs-lookup"><span data-stu-id="d07ef-124">value</span></span>|<span data-ttu-id="d07ef-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d07ef-125">Int32</span></span>|<span data-ttu-id="d07ef-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="d07ef-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d07ef-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d07ef-127">Relationships</span></span>
<span data-ttu-id="d07ef-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d07ef-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d07ef-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d07ef-129">JSON Representation</span></span>
<span data-ttu-id="d07ef-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d07ef-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```




