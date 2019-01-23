---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82ab4c5aaab700b08a0af95e47010f3d06b79b04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410821"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="fd89a-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="fd89a-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="fd89a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd89a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fd89a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd89a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd89a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd89a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd89a-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="fd89a-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="fd89a-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd89a-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd89a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd89a-109">Properties</span></span>
|<span data-ttu-id="fd89a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd89a-110">Property</span></span>|<span data-ttu-id="fd89a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fd89a-111">Type</span></span>|<span data-ttu-id="fd89a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fd89a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd89a-113">displayName</span><span class="sxs-lookup"><span data-stu-id="fd89a-113">displayName</span></span>|<span data-ttu-id="fd89a-114">String</span><span class="sxs-lookup"><span data-stu-id="fd89a-114">String</span></span>|<span data-ttu-id="fd89a-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fd89a-115">Display Name.</span></span> <span data-ttu-id="fd89a-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd89a-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd89a-117">description</span><span class="sxs-lookup"><span data-stu-id="fd89a-117">description</span></span>|<span data-ttu-id="fd89a-118">String</span><span class="sxs-lookup"><span data-stu-id="fd89a-118">String</span></span>|<span data-ttu-id="fd89a-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="fd89a-119">Description.</span></span> <span data-ttu-id="fd89a-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd89a-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd89a-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="fd89a-121">omaUri</span></span>|<span data-ttu-id="fd89a-122">String</span><span class="sxs-lookup"><span data-stu-id="fd89a-122">String</span></span>|<span data-ttu-id="fd89a-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="fd89a-123">OMA.</span></span> <span data-ttu-id="fd89a-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd89a-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fd89a-125">value</span><span class="sxs-lookup"><span data-stu-id="fd89a-125">value</span></span>|<span data-ttu-id="fd89a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd89a-126">DateTimeOffset</span></span>|<span data-ttu-id="fd89a-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="fd89a-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd89a-128">Связи</span><span class="sxs-lookup"><span data-stu-id="fd89a-128">Relationships</span></span>
<span data-ttu-id="fd89a-129">Нет</span><span class="sxs-lookup"><span data-stu-id="fd89a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd89a-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd89a-130">JSON Representation</span></span>
<span data-ttu-id="fd89a-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd89a-131">Here is a JSON representation of the resource.</span></span>
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




