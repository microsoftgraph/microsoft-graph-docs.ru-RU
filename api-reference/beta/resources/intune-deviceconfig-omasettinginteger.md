---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64fbfca7b5fc101ea7ea64d4545257354d4157e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010173"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="a3111-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="a3111-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="a3111-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3111-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3111-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3111-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3111-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3111-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3111-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="a3111-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="a3111-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a3111-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a3111-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3111-109">Properties</span></span>
|<span data-ttu-id="a3111-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3111-110">Property</span></span>|<span data-ttu-id="a3111-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a3111-111">Type</span></span>|<span data-ttu-id="a3111-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a3111-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3111-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a3111-113">displayName</span></span>|<span data-ttu-id="a3111-114">String</span><span class="sxs-lookup"><span data-stu-id="a3111-114">String</span></span>|<span data-ttu-id="a3111-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a3111-115">Display Name.</span></span> <span data-ttu-id="a3111-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a3111-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a3111-117">description</span><span class="sxs-lookup"><span data-stu-id="a3111-117">description</span></span>|<span data-ttu-id="a3111-118">String</span><span class="sxs-lookup"><span data-stu-id="a3111-118">String</span></span>|<span data-ttu-id="a3111-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="a3111-119">Description.</span></span> <span data-ttu-id="a3111-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a3111-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a3111-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="a3111-121">omaUri</span></span>|<span data-ttu-id="a3111-122">String</span><span class="sxs-lookup"><span data-stu-id="a3111-122">String</span></span>|<span data-ttu-id="a3111-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="a3111-123">OMA.</span></span> <span data-ttu-id="a3111-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a3111-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a3111-125">value</span><span class="sxs-lookup"><span data-stu-id="a3111-125">value</span></span>|<span data-ttu-id="a3111-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a3111-126">Int32</span></span>|<span data-ttu-id="a3111-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="a3111-127">Value.</span></span>|
|<span data-ttu-id="a3111-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="a3111-128">isReadOnly</span></span>|<span data-ttu-id="a3111-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3111-129">Boolean</span></span>|<span data-ttu-id="a3111-130">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="a3111-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3111-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="a3111-131">Relationships</span></span>
<span data-ttu-id="a3111-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a3111-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3111-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3111-133">JSON Representation</span></span>
<span data-ttu-id="a3111-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3111-134">Here is a JSON representation of the resource.</span></span>
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
  "value": 1024,
  "isReadOnly": true
}
```






