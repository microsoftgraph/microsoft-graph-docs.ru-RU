---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dabc0f58836f240d229049befe9055fc87e57b2a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068996"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="aa54b-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="aa54b-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="aa54b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa54b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa54b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa54b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa54b-106">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="aa54b-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="aa54b-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aa54b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa54b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa54b-108">Properties</span></span>
|<span data-ttu-id="aa54b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa54b-109">Property</span></span>|<span data-ttu-id="aa54b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aa54b-110">Type</span></span>|<span data-ttu-id="aa54b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aa54b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa54b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="aa54b-112">displayName</span></span>|<span data-ttu-id="aa54b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="aa54b-113">String</span></span>|<span data-ttu-id="aa54b-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="aa54b-114">Display Name.</span></span> <span data-ttu-id="aa54b-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aa54b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aa54b-116">description</span><span class="sxs-lookup"><span data-stu-id="aa54b-116">description</span></span>|<span data-ttu-id="aa54b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="aa54b-117">String</span></span>|<span data-ttu-id="aa54b-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="aa54b-118">Description.</span></span> <span data-ttu-id="aa54b-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aa54b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aa54b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="aa54b-120">omaUri</span></span>|<span data-ttu-id="aa54b-121">String</span><span class="sxs-lookup"><span data-stu-id="aa54b-121">String</span></span>|<span data-ttu-id="aa54b-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="aa54b-122">OMA.</span></span> <span data-ttu-id="aa54b-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="aa54b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="aa54b-124">value</span><span class="sxs-lookup"><span data-stu-id="aa54b-124">value</span></span>|<span data-ttu-id="aa54b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa54b-125">Boolean</span></span>|<span data-ttu-id="aa54b-126">Значение</span><span class="sxs-lookup"><span data-stu-id="aa54b-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa54b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="aa54b-127">Relationships</span></span>
<span data-ttu-id="aa54b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="aa54b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa54b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa54b-129">JSON Representation</span></span>
<span data-ttu-id="aa54b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa54b-130">Here is a JSON representation of the resource.</span></span>
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









