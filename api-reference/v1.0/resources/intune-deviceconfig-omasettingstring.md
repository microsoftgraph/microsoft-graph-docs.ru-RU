---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05f37b94aecadd5e3da1d0e162cd8bf6afe96681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988270"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="309b0-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="309b0-103">omaSettingString resource type</span></span>

<span data-ttu-id="309b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="309b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="309b0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="309b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="309b0-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="309b0-106">OMA Settings String definition.</span></span>


<span data-ttu-id="309b0-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="309b0-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="309b0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="309b0-108">Properties</span></span>
|<span data-ttu-id="309b0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="309b0-109">Property</span></span>|<span data-ttu-id="309b0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="309b0-110">Type</span></span>|<span data-ttu-id="309b0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="309b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="309b0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="309b0-112">displayName</span></span>|<span data-ttu-id="309b0-113">String</span><span class="sxs-lookup"><span data-stu-id="309b0-113">String</span></span>|<span data-ttu-id="309b0-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="309b0-114">Display Name.</span></span> <span data-ttu-id="309b0-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="309b0-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="309b0-116">description</span><span class="sxs-lookup"><span data-stu-id="309b0-116">description</span></span>|<span data-ttu-id="309b0-117">String</span><span class="sxs-lookup"><span data-stu-id="309b0-117">String</span></span>|<span data-ttu-id="309b0-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="309b0-118">Description.</span></span> <span data-ttu-id="309b0-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="309b0-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="309b0-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="309b0-120">omaUri</span></span>|<span data-ttu-id="309b0-121">String</span><span class="sxs-lookup"><span data-stu-id="309b0-121">String</span></span>|<span data-ttu-id="309b0-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="309b0-122">OMA.</span></span> <span data-ttu-id="309b0-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="309b0-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="309b0-124">value</span><span class="sxs-lookup"><span data-stu-id="309b0-124">value</span></span>|<span data-ttu-id="309b0-125">String</span><span class="sxs-lookup"><span data-stu-id="309b0-125">String</span></span>|<span data-ttu-id="309b0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="309b0-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="309b0-127">Связи</span><span class="sxs-lookup"><span data-stu-id="309b0-127">Relationships</span></span>
<span data-ttu-id="309b0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="309b0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="309b0-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="309b0-129">JSON Representation</span></span>
<span data-ttu-id="309b0-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="309b0-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```









