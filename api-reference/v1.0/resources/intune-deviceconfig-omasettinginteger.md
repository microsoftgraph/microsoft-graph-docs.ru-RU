---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569020"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="3bde3-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="3bde3-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="3bde3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3bde3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bde3-105">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="3bde3-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="3bde3-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3bde3-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3bde3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3bde3-107">Properties</span></span>
|<span data-ttu-id="3bde3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bde3-108">Property</span></span>|<span data-ttu-id="3bde3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3bde3-109">Type</span></span>|<span data-ttu-id="3bde3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3bde3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bde3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3bde3-111">displayName</span></span>|<span data-ttu-id="3bde3-112">String</span><span class="sxs-lookup"><span data-stu-id="3bde3-112">String</span></span>|<span data-ttu-id="3bde3-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3bde3-113">Display Name.</span></span> <span data-ttu-id="3bde3-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3bde3-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3bde3-115">description</span><span class="sxs-lookup"><span data-stu-id="3bde3-115">description</span></span>|<span data-ttu-id="3bde3-116">String</span><span class="sxs-lookup"><span data-stu-id="3bde3-116">String</span></span>|<span data-ttu-id="3bde3-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="3bde3-117">Description.</span></span> <span data-ttu-id="3bde3-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3bde3-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3bde3-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="3bde3-119">omaUri</span></span>|<span data-ttu-id="3bde3-120">String</span><span class="sxs-lookup"><span data-stu-id="3bde3-120">String</span></span>|<span data-ttu-id="3bde3-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="3bde3-121">OMA.</span></span> <span data-ttu-id="3bde3-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3bde3-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3bde3-123">value</span><span class="sxs-lookup"><span data-stu-id="3bde3-123">value</span></span>|<span data-ttu-id="3bde3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3bde3-124">Int32</span></span>|<span data-ttu-id="3bde3-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="3bde3-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bde3-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="3bde3-126">Relationships</span></span>
<span data-ttu-id="3bde3-127">Нет</span><span class="sxs-lookup"><span data-stu-id="3bde3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bde3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3bde3-128">JSON Representation</span></span>
<span data-ttu-id="3bde3-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bde3-129">Here is a JSON representation of the resource.</span></span>
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



