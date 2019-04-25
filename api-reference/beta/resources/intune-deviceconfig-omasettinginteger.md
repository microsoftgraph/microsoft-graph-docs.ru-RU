---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54eec27cf91bb1da7790ae1432452ac026bf1683
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542125"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="45ea3-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="45ea3-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="45ea3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45ea3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ea3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45ea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ea3-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="45ea3-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="45ea3-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45ea3-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45ea3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="45ea3-108">Properties</span></span>
|<span data-ttu-id="45ea3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="45ea3-109">Property</span></span>|<span data-ttu-id="45ea3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="45ea3-110">Type</span></span>|<span data-ttu-id="45ea3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="45ea3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ea3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="45ea3-112">displayName</span></span>|<span data-ttu-id="45ea3-113">String</span><span class="sxs-lookup"><span data-stu-id="45ea3-113">String</span></span>|<span data-ttu-id="45ea3-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="45ea3-114">Display Name.</span></span> <span data-ttu-id="45ea3-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45ea3-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45ea3-116">description</span><span class="sxs-lookup"><span data-stu-id="45ea3-116">description</span></span>|<span data-ttu-id="45ea3-117">String</span><span class="sxs-lookup"><span data-stu-id="45ea3-117">String</span></span>|<span data-ttu-id="45ea3-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="45ea3-118">Description.</span></span> <span data-ttu-id="45ea3-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45ea3-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45ea3-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="45ea3-120">omaUri</span></span>|<span data-ttu-id="45ea3-121">String</span><span class="sxs-lookup"><span data-stu-id="45ea3-121">String</span></span>|<span data-ttu-id="45ea3-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="45ea3-122">OMA.</span></span> <span data-ttu-id="45ea3-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="45ea3-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="45ea3-124">value</span><span class="sxs-lookup"><span data-stu-id="45ea3-124">value</span></span>|<span data-ttu-id="45ea3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="45ea3-125">Int32</span></span>|<span data-ttu-id="45ea3-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="45ea3-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45ea3-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="45ea3-127">Relationships</span></span>
<span data-ttu-id="45ea3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="45ea3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45ea3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45ea3-129">JSON Representation</span></span>
<span data-ttu-id="45ea3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45ea3-130">Here is a JSON representation of the resource.</span></span>
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





