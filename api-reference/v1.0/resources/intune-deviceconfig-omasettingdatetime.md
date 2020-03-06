---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c85711df4d7de9245196ca86ea47de0c72efc9c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532430"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d0723-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="d0723-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="d0723-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0723-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0723-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0723-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0723-106">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="d0723-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="d0723-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0723-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0723-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0723-108">Properties</span></span>
|<span data-ttu-id="d0723-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0723-109">Property</span></span>|<span data-ttu-id="d0723-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d0723-110">Type</span></span>|<span data-ttu-id="d0723-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d0723-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0723-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d0723-112">displayName</span></span>|<span data-ttu-id="d0723-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d0723-113">String</span></span>|<span data-ttu-id="d0723-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="d0723-114">Display Name.</span></span> <span data-ttu-id="d0723-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0723-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d0723-116">description</span><span class="sxs-lookup"><span data-stu-id="d0723-116">description</span></span>|<span data-ttu-id="d0723-117">String</span><span class="sxs-lookup"><span data-stu-id="d0723-117">String</span></span>|<span data-ttu-id="d0723-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="d0723-118">Description.</span></span> <span data-ttu-id="d0723-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0723-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d0723-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d0723-120">omaUri</span></span>|<span data-ttu-id="d0723-121">String</span><span class="sxs-lookup"><span data-stu-id="d0723-121">String</span></span>|<span data-ttu-id="d0723-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="d0723-122">OMA.</span></span> <span data-ttu-id="d0723-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d0723-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d0723-124">value</span><span class="sxs-lookup"><span data-stu-id="d0723-124">value</span></span>|<span data-ttu-id="d0723-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0723-125">DateTimeOffset</span></span>|<span data-ttu-id="d0723-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="d0723-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0723-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d0723-127">Relationships</span></span>
<span data-ttu-id="d0723-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d0723-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0723-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0723-129">JSON Representation</span></span>
<span data-ttu-id="d0723-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0723-130">Here is a JSON representation of the resource.</span></span>
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




