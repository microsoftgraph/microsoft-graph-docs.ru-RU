---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7269b8c61603601d0932a000f7f90e63d7cbc44e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993734"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="3ac55-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="3ac55-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="3ac55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ac55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ac55-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ac55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ac55-106">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="3ac55-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="3ac55-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ac55-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ac55-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ac55-108">Properties</span></span>
|<span data-ttu-id="3ac55-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ac55-109">Property</span></span>|<span data-ttu-id="3ac55-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ac55-110">Type</span></span>|<span data-ttu-id="3ac55-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ac55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ac55-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3ac55-112">displayName</span></span>|<span data-ttu-id="3ac55-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3ac55-113">String</span></span>|<span data-ttu-id="3ac55-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3ac55-114">Display Name.</span></span> <span data-ttu-id="3ac55-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ac55-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ac55-116">description</span><span class="sxs-lookup"><span data-stu-id="3ac55-116">description</span></span>|<span data-ttu-id="3ac55-117">String</span><span class="sxs-lookup"><span data-stu-id="3ac55-117">String</span></span>|<span data-ttu-id="3ac55-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="3ac55-118">Description.</span></span> <span data-ttu-id="3ac55-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ac55-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ac55-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3ac55-120">omaUri</span></span>|<span data-ttu-id="3ac55-121">String</span><span class="sxs-lookup"><span data-stu-id="3ac55-121">String</span></span>|<span data-ttu-id="3ac55-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="3ac55-122">OMA.</span></span> <span data-ttu-id="3ac55-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3ac55-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3ac55-124">value</span><span class="sxs-lookup"><span data-stu-id="3ac55-124">value</span></span>|<span data-ttu-id="3ac55-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ac55-125">Boolean</span></span>|<span data-ttu-id="3ac55-126">Значение</span><span class="sxs-lookup"><span data-stu-id="3ac55-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ac55-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ac55-127">Relationships</span></span>
<span data-ttu-id="3ac55-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3ac55-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ac55-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ac55-129">JSON Representation</span></span>
<span data-ttu-id="3ac55-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ac55-130">Here is a JSON representation of the resource.</span></span>
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





