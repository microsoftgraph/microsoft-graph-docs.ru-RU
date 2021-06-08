---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3674e9d7efb438f5afb18e6fdb5b46a261086236
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760246"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="4fa21-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="4fa21-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="4fa21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fa21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fa21-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fa21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fa21-106">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="4fa21-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="4fa21-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4fa21-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4fa21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fa21-108">Properties</span></span>
|<span data-ttu-id="4fa21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fa21-109">Property</span></span>|<span data-ttu-id="4fa21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4fa21-110">Type</span></span>|<span data-ttu-id="4fa21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4fa21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa21-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4fa21-112">displayName</span></span>|<span data-ttu-id="4fa21-113">String</span><span class="sxs-lookup"><span data-stu-id="4fa21-113">String</span></span>|<span data-ttu-id="4fa21-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4fa21-114">Display Name.</span></span> <span data-ttu-id="4fa21-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4fa21-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4fa21-116">description</span><span class="sxs-lookup"><span data-stu-id="4fa21-116">description</span></span>|<span data-ttu-id="4fa21-117">String</span><span class="sxs-lookup"><span data-stu-id="4fa21-117">String</span></span>|<span data-ttu-id="4fa21-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="4fa21-118">Description.</span></span> <span data-ttu-id="4fa21-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4fa21-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4fa21-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="4fa21-120">omaUri</span></span>|<span data-ttu-id="4fa21-121">String</span><span class="sxs-lookup"><span data-stu-id="4fa21-121">String</span></span>|<span data-ttu-id="4fa21-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="4fa21-122">OMA.</span></span> <span data-ttu-id="4fa21-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4fa21-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4fa21-124">value</span><span class="sxs-lookup"><span data-stu-id="4fa21-124">value</span></span>|<span data-ttu-id="4fa21-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fa21-125">Boolean</span></span>|<span data-ttu-id="4fa21-126">Значение</span><span class="sxs-lookup"><span data-stu-id="4fa21-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fa21-127">Связи</span><span class="sxs-lookup"><span data-stu-id="4fa21-127">Relationships</span></span>
<span data-ttu-id="4fa21-128">Нет</span><span class="sxs-lookup"><span data-stu-id="4fa21-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fa21-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fa21-129">JSON Representation</span></span>
<span data-ttu-id="4fa21-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fa21-130">Here is a JSON representation of the resource.</span></span>
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




