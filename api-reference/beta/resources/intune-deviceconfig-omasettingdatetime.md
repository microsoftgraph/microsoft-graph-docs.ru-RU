---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a237f36a209e2fa1d552c8f50207770429a0c53
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554494"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="712a0-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="712a0-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="712a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="712a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="712a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="712a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="712a0-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="712a0-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="712a0-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="712a0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="712a0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="712a0-108">Properties</span></span>
|<span data-ttu-id="712a0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="712a0-109">Property</span></span>|<span data-ttu-id="712a0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="712a0-110">Type</span></span>|<span data-ttu-id="712a0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="712a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="712a0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="712a0-112">displayName</span></span>|<span data-ttu-id="712a0-113">String</span><span class="sxs-lookup"><span data-stu-id="712a0-113">String</span></span>|<span data-ttu-id="712a0-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="712a0-114">Display Name.</span></span> <span data-ttu-id="712a0-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="712a0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="712a0-116">description</span><span class="sxs-lookup"><span data-stu-id="712a0-116">description</span></span>|<span data-ttu-id="712a0-117">String</span><span class="sxs-lookup"><span data-stu-id="712a0-117">String</span></span>|<span data-ttu-id="712a0-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="712a0-118">Description.</span></span> <span data-ttu-id="712a0-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="712a0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="712a0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="712a0-120">omaUri</span></span>|<span data-ttu-id="712a0-121">String</span><span class="sxs-lookup"><span data-stu-id="712a0-121">String</span></span>|<span data-ttu-id="712a0-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="712a0-122">OMA.</span></span> <span data-ttu-id="712a0-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="712a0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="712a0-124">value</span><span class="sxs-lookup"><span data-stu-id="712a0-124">value</span></span>|<span data-ttu-id="712a0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="712a0-125">DateTimeOffset</span></span>|<span data-ttu-id="712a0-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="712a0-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="712a0-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="712a0-127">Relationships</span></span>
<span data-ttu-id="712a0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="712a0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="712a0-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="712a0-129">JSON Representation</span></span>
<span data-ttu-id="712a0-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="712a0-130">Here is a JSON representation of the resource.</span></span>
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





