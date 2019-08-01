---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 122a8fd7ffdef7d314e16bf6154838e09598f7d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031320"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="c2a76-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="c2a76-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="c2a76-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2a76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2a76-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c2a76-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="c2a76-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2a76-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2a76-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2a76-107">Properties</span></span>
|<span data-ttu-id="c2a76-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2a76-108">Property</span></span>|<span data-ttu-id="c2a76-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2a76-109">Type</span></span>|<span data-ttu-id="c2a76-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2a76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2a76-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c2a76-111">displayName</span></span>|<span data-ttu-id="c2a76-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c2a76-112">String</span></span>|<span data-ttu-id="c2a76-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c2a76-113">Display Name.</span></span> <span data-ttu-id="c2a76-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2a76-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2a76-115">description</span><span class="sxs-lookup"><span data-stu-id="c2a76-115">description</span></span>|<span data-ttu-id="c2a76-116">String</span><span class="sxs-lookup"><span data-stu-id="c2a76-116">String</span></span>|<span data-ttu-id="c2a76-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="c2a76-117">Description.</span></span> <span data-ttu-id="c2a76-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2a76-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2a76-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="c2a76-119">omaUri</span></span>|<span data-ttu-id="c2a76-120">String</span><span class="sxs-lookup"><span data-stu-id="c2a76-120">String</span></span>|<span data-ttu-id="c2a76-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="c2a76-121">OMA.</span></span> <span data-ttu-id="c2a76-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c2a76-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c2a76-123">value</span><span class="sxs-lookup"><span data-stu-id="c2a76-123">value</span></span>|<span data-ttu-id="c2a76-124">Single</span><span class="sxs-lookup"><span data-stu-id="c2a76-124">Single</span></span>|<span data-ttu-id="c2a76-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="c2a76-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2a76-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="c2a76-126">Relationships</span></span>
<span data-ttu-id="c2a76-127">Нет</span><span class="sxs-lookup"><span data-stu-id="c2a76-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2a76-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2a76-128">JSON Representation</span></span>
<span data-ttu-id="c2a76-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2a76-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



