---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0ecb59f45a83cc98c6ff060b46ba0c620dc9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031341"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="5e926-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="5e926-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="5e926-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e926-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e926-105">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="5e926-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="5e926-106">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5e926-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e926-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e926-107">Properties</span></span>
|<span data-ttu-id="5e926-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e926-108">Property</span></span>|<span data-ttu-id="5e926-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e926-109">Type</span></span>|<span data-ttu-id="5e926-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e926-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e926-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5e926-111">displayName</span></span>|<span data-ttu-id="5e926-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5e926-112">String</span></span>|<span data-ttu-id="5e926-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="5e926-113">Display Name.</span></span> <span data-ttu-id="5e926-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5e926-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5e926-115">description</span><span class="sxs-lookup"><span data-stu-id="5e926-115">description</span></span>|<span data-ttu-id="5e926-116">String</span><span class="sxs-lookup"><span data-stu-id="5e926-116">String</span></span>|<span data-ttu-id="5e926-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="5e926-117">Description.</span></span> <span data-ttu-id="5e926-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5e926-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5e926-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="5e926-119">omaUri</span></span>|<span data-ttu-id="5e926-120">String</span><span class="sxs-lookup"><span data-stu-id="5e926-120">String</span></span>|<span data-ttu-id="5e926-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="5e926-121">OMA.</span></span> <span data-ttu-id="5e926-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5e926-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5e926-123">value</span><span class="sxs-lookup"><span data-stu-id="5e926-123">value</span></span>|<span data-ttu-id="5e926-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e926-124">Boolean</span></span>|<span data-ttu-id="5e926-125">Значение</span><span class="sxs-lookup"><span data-stu-id="5e926-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e926-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e926-126">Relationships</span></span>
<span data-ttu-id="5e926-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5e926-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e926-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e926-128">JSON Representation</span></span>
<span data-ttu-id="5e926-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e926-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



