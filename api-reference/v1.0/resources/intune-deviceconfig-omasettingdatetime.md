---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d8d9151ad40ef42ca24730197cdebe882eccb97
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473043"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="6a037-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="6a037-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="6a037-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a037-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a037-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a037-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="6a037-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="6a037-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6a037-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a037-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a037-108">Properties</span></span>
|<span data-ttu-id="6a037-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a037-109">Property</span></span>|<span data-ttu-id="6a037-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a037-110">Type</span></span>|<span data-ttu-id="6a037-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a037-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a037-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6a037-112">displayName</span></span>|<span data-ttu-id="6a037-113">Строка</span><span class="sxs-lookup"><span data-stu-id="6a037-113">String</span></span>|<span data-ttu-id="6a037-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="6a037-114">Display Name.</span></span> <span data-ttu-id="6a037-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6a037-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6a037-116">description</span><span class="sxs-lookup"><span data-stu-id="6a037-116">description</span></span>|<span data-ttu-id="6a037-117">String</span><span class="sxs-lookup"><span data-stu-id="6a037-117">String</span></span>|<span data-ttu-id="6a037-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="6a037-118">Description.</span></span> <span data-ttu-id="6a037-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6a037-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6a037-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="6a037-120">omaUri</span></span>|<span data-ttu-id="6a037-121">String</span><span class="sxs-lookup"><span data-stu-id="6a037-121">String</span></span>|<span data-ttu-id="6a037-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="6a037-122">OMA.</span></span> <span data-ttu-id="6a037-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6a037-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6a037-124">value</span><span class="sxs-lookup"><span data-stu-id="6a037-124">value</span></span>|<span data-ttu-id="6a037-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a037-125">DateTimeOffset</span></span>|<span data-ttu-id="6a037-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="6a037-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a037-127">Связи</span><span class="sxs-lookup"><span data-stu-id="6a037-127">Relationships</span></span>
<span data-ttu-id="6a037-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6a037-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a037-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a037-129">JSON Representation</span></span>
<span data-ttu-id="6a037-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a037-130">Here is a JSON representation of the resource.</span></span>
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







