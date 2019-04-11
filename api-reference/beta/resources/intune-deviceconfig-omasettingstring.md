---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22c69270126349d8d1d4afca4555abd18768aa3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803033"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="dca81-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="dca81-103">omaSettingString resource type</span></span>

> <span data-ttu-id="dca81-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca81-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dca81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca81-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="dca81-106">OMA Settings String definition.</span></span>


<span data-ttu-id="dca81-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca81-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dca81-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dca81-108">Properties</span></span>
|<span data-ttu-id="dca81-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca81-109">Property</span></span>|<span data-ttu-id="dca81-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dca81-110">Type</span></span>|<span data-ttu-id="dca81-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dca81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca81-112">displayName</span><span class="sxs-lookup"><span data-stu-id="dca81-112">displayName</span></span>|<span data-ttu-id="dca81-113">String</span><span class="sxs-lookup"><span data-stu-id="dca81-113">String</span></span>|<span data-ttu-id="dca81-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="dca81-114">Display Name.</span></span> <span data-ttu-id="dca81-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca81-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca81-116">description</span><span class="sxs-lookup"><span data-stu-id="dca81-116">description</span></span>|<span data-ttu-id="dca81-117">String</span><span class="sxs-lookup"><span data-stu-id="dca81-117">String</span></span>|<span data-ttu-id="dca81-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="dca81-118">Description.</span></span> <span data-ttu-id="dca81-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca81-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca81-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="dca81-120">omaUri</span></span>|<span data-ttu-id="dca81-121">String</span><span class="sxs-lookup"><span data-stu-id="dca81-121">String</span></span>|<span data-ttu-id="dca81-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="dca81-122">OMA.</span></span> <span data-ttu-id="dca81-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca81-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca81-124">value</span><span class="sxs-lookup"><span data-stu-id="dca81-124">value</span></span>|<span data-ttu-id="dca81-125">Строка</span><span class="sxs-lookup"><span data-stu-id="dca81-125">String</span></span>|<span data-ttu-id="dca81-126">Значение</span><span class="sxs-lookup"><span data-stu-id="dca81-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca81-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="dca81-127">Relationships</span></span>
<span data-ttu-id="dca81-128">Нет</span><span class="sxs-lookup"><span data-stu-id="dca81-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca81-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dca81-129">JSON Representation</span></span>
<span data-ttu-id="dca81-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca81-130">Here is a JSON representation of the resource.</span></span>
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





