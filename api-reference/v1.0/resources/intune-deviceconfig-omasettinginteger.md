---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46406b403dd700ee7e8517c10956f310957dcaf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978162"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="0f734-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="0f734-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="0f734-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f734-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f734-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f734-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f734-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0f734-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="0f734-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f734-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f734-108">Properties</span></span>
|<span data-ttu-id="0f734-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f734-109">Property</span></span>|<span data-ttu-id="0f734-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f734-110">Type</span></span>|<span data-ttu-id="0f734-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f734-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f734-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0f734-112">displayName</span></span>|<span data-ttu-id="0f734-113">String</span><span class="sxs-lookup"><span data-stu-id="0f734-113">String</span></span>|<span data-ttu-id="0f734-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0f734-114">Display Name.</span></span> <span data-ttu-id="0f734-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f734-116">description</span><span class="sxs-lookup"><span data-stu-id="0f734-116">description</span></span>|<span data-ttu-id="0f734-117">String</span><span class="sxs-lookup"><span data-stu-id="0f734-117">String</span></span>|<span data-ttu-id="0f734-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="0f734-118">Description.</span></span> <span data-ttu-id="0f734-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f734-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="0f734-120">omaUri</span></span>|<span data-ttu-id="0f734-121">String</span><span class="sxs-lookup"><span data-stu-id="0f734-121">String</span></span>|<span data-ttu-id="0f734-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="0f734-122">OMA.</span></span> <span data-ttu-id="0f734-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0f734-124">value</span><span class="sxs-lookup"><span data-stu-id="0f734-124">value</span></span>|<span data-ttu-id="0f734-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-125">Int32</span></span>|<span data-ttu-id="0f734-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="0f734-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f734-127">Связи</span><span class="sxs-lookup"><span data-stu-id="0f734-127">Relationships</span></span>
<span data-ttu-id="0f734-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0f734-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f734-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f734-129">JSON Representation</span></span>
<span data-ttu-id="0f734-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f734-130">Here is a JSON representation of the resource.</span></span>
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









