---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d4ade59cc6359f4cc9f5bd668882860cf49ff49
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788459"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d232f-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="d232f-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="d232f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d232f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d232f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d232f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d232f-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d232f-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="d232f-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d232f-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d232f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d232f-108">Properties</span></span>
|<span data-ttu-id="d232f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d232f-109">Property</span></span>|<span data-ttu-id="d232f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d232f-110">Type</span></span>|<span data-ttu-id="d232f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d232f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d232f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d232f-112">displayName</span></span>|<span data-ttu-id="d232f-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d232f-113">String</span></span>|<span data-ttu-id="d232f-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d232f-114">Display Name.</span></span> <span data-ttu-id="d232f-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d232f-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d232f-116">description</span><span class="sxs-lookup"><span data-stu-id="d232f-116">description</span></span>|<span data-ttu-id="d232f-117">String</span><span class="sxs-lookup"><span data-stu-id="d232f-117">String</span></span>|<span data-ttu-id="d232f-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="d232f-118">Description.</span></span> <span data-ttu-id="d232f-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d232f-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d232f-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d232f-120">omaUri</span></span>|<span data-ttu-id="d232f-121">String</span><span class="sxs-lookup"><span data-stu-id="d232f-121">String</span></span>|<span data-ttu-id="d232f-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d232f-122">OMA.</span></span> <span data-ttu-id="d232f-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d232f-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d232f-124">value</span><span class="sxs-lookup"><span data-stu-id="d232f-124">value</span></span>|<span data-ttu-id="d232f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d232f-125">DateTimeOffset</span></span>|<span data-ttu-id="d232f-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="d232f-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d232f-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d232f-127">Relationships</span></span>
<span data-ttu-id="d232f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d232f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d232f-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d232f-129">JSON Representation</span></span>
<span data-ttu-id="d232f-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d232f-130">Here is a JSON representation of the resource.</span></span>
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



