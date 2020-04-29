---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cf2e556fe434a7a0ab8baa4d42a4098e66c698cd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473006"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="34bf2-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="34bf2-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="34bf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34bf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34bf2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34bf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bf2-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="34bf2-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="34bf2-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34bf2-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34bf2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="34bf2-108">Properties</span></span>
|<span data-ttu-id="34bf2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="34bf2-109">Property</span></span>|<span data-ttu-id="34bf2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="34bf2-110">Type</span></span>|<span data-ttu-id="34bf2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34bf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34bf2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="34bf2-112">displayName</span></span>|<span data-ttu-id="34bf2-113">Строка</span><span class="sxs-lookup"><span data-stu-id="34bf2-113">String</span></span>|<span data-ttu-id="34bf2-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="34bf2-114">Display Name.</span></span> <span data-ttu-id="34bf2-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34bf2-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="34bf2-116">description</span><span class="sxs-lookup"><span data-stu-id="34bf2-116">description</span></span>|<span data-ttu-id="34bf2-117">String</span><span class="sxs-lookup"><span data-stu-id="34bf2-117">String</span></span>|<span data-ttu-id="34bf2-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="34bf2-118">Description.</span></span> <span data-ttu-id="34bf2-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34bf2-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="34bf2-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="34bf2-120">omaUri</span></span>|<span data-ttu-id="34bf2-121">String</span><span class="sxs-lookup"><span data-stu-id="34bf2-121">String</span></span>|<span data-ttu-id="34bf2-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="34bf2-122">OMA.</span></span> <span data-ttu-id="34bf2-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34bf2-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="34bf2-124">value</span><span class="sxs-lookup"><span data-stu-id="34bf2-124">value</span></span>|<span data-ttu-id="34bf2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="34bf2-125">Int32</span></span>|<span data-ttu-id="34bf2-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="34bf2-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34bf2-127">Связи</span><span class="sxs-lookup"><span data-stu-id="34bf2-127">Relationships</span></span>
<span data-ttu-id="34bf2-128">Нет</span><span class="sxs-lookup"><span data-stu-id="34bf2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34bf2-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34bf2-129">JSON Representation</span></span>
<span data-ttu-id="34bf2-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34bf2-130">Here is a JSON representation of the resource.</span></span>
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







