---
title: Тип ресурса omaSettingDateTime
description: Определение даты и времени параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1b5ed3498728fbdc99602b0bd9953315e76e02b0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273139"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="ff919-103">Тип ресурса omaSettingDateTime</span><span class="sxs-lookup"><span data-stu-id="ff919-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="ff919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff919-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff919-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff919-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff919-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff919-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff919-107">Определение даты и времени параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="ff919-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="ff919-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff919-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff919-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff919-109">Properties</span></span>
|<span data-ttu-id="ff919-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff919-110">Property</span></span>|<span data-ttu-id="ff919-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff919-111">Type</span></span>|<span data-ttu-id="ff919-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff919-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff919-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ff919-113">displayName</span></span>|<span data-ttu-id="ff919-114">String</span><span class="sxs-lookup"><span data-stu-id="ff919-114">String</span></span>|<span data-ttu-id="ff919-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="ff919-115">Display Name.</span></span> <span data-ttu-id="ff919-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff919-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff919-117">description</span><span class="sxs-lookup"><span data-stu-id="ff919-117">description</span></span>|<span data-ttu-id="ff919-118">String</span><span class="sxs-lookup"><span data-stu-id="ff919-118">String</span></span>|<span data-ttu-id="ff919-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="ff919-119">Description.</span></span> <span data-ttu-id="ff919-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff919-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff919-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ff919-121">omaUri</span></span>|<span data-ttu-id="ff919-122">String</span><span class="sxs-lookup"><span data-stu-id="ff919-122">String</span></span>|<span data-ttu-id="ff919-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="ff919-123">OMA.</span></span> <span data-ttu-id="ff919-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff919-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff919-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ff919-125">isEncrypted</span></span>|<span data-ttu-id="ff919-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff919-126">Boolean</span></span>|<span data-ttu-id="ff919-127">Указывает, зашифровано ли поле "значение".</span><span class="sxs-lookup"><span data-stu-id="ff919-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="ff919-128">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ff919-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ff919-129">value</span><span class="sxs-lookup"><span data-stu-id="ff919-129">value</span></span>|<span data-ttu-id="ff919-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff919-130">DateTimeOffset</span></span>|<span data-ttu-id="ff919-131">Значение.</span><span class="sxs-lookup"><span data-stu-id="ff919-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff919-132">Связи</span><span class="sxs-lookup"><span data-stu-id="ff919-132">Relationships</span></span>
<span data-ttu-id="ff919-133">Нет</span><span class="sxs-lookup"><span data-stu-id="ff919-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff919-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff919-134">JSON Representation</span></span>
<span data-ttu-id="ff919-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff919-135">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "value": "String (timestamp)"
}
```




