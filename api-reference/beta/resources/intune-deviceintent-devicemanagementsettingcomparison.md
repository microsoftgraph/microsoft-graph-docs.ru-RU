---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a91dc3ce4cb7e8730f346800d53740db78e5526
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785353"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="fc377-103">Тип ресурса Девицеманажементсеттингкомпарисон</span><span class="sxs-lookup"><span data-stu-id="fc377-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="fc377-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc377-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc377-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc377-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc377-106">Объект, представляющий результат сравнения параметров</span><span class="sxs-lookup"><span data-stu-id="fc377-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="fc377-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc377-107">Properties</span></span>
|<span data-ttu-id="fc377-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc377-108">Property</span></span>|<span data-ttu-id="fc377-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc377-109">Type</span></span>|<span data-ttu-id="fc377-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc377-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc377-111">id</span><span class="sxs-lookup"><span data-stu-id="fc377-111">id</span></span>|<span data-ttu-id="fc377-112">String</span><span class="sxs-lookup"><span data-stu-id="fc377-112">String</span></span>|<span data-ttu-id="fc377-113">Идентификатор параметра</span><span class="sxs-lookup"><span data-stu-id="fc377-113">The setting ID</span></span>|
|<span data-ttu-id="fc377-114">displayName</span><span class="sxs-lookup"><span data-stu-id="fc377-114">displayName</span></span>|<span data-ttu-id="fc377-115">Строка</span><span class="sxs-lookup"><span data-stu-id="fc377-115">String</span></span>|<span data-ttu-id="fc377-116">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="fc377-116">The setting's display name</span></span>|
|<span data-ttu-id="fc377-117">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="fc377-117">definitionId</span></span>|<span data-ttu-id="fc377-118">String</span><span class="sxs-lookup"><span data-stu-id="fc377-118">String</span></span>|<span data-ttu-id="fc377-119">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="fc377-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="fc377-120">куррентвалуежсон</span><span class="sxs-lookup"><span data-stu-id="fc377-120">currentValueJson</span></span>|<span data-ttu-id="fc377-121">String</span><span class="sxs-lookup"><span data-stu-id="fc377-121">String</span></span>|<span data-ttu-id="fc377-122">Значение параметра шаблона (или) в формате JSON для текущего способа (или)</span><span class="sxs-lookup"><span data-stu-id="fc377-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="fc377-123">неввалуежсон</span><span class="sxs-lookup"><span data-stu-id="fc377-123">newValueJson</span></span>|<span data-ttu-id="fc377-124">String</span><span class="sxs-lookup"><span data-stu-id="fc377-124">String</span></span>|<span data-ttu-id="fc377-125">Представление нового значения параметра шаблона в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc377-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="fc377-126">компарисонресулт</span><span class="sxs-lookup"><span data-stu-id="fc377-126">comparisonResult</span></span>|[<span data-ttu-id="fc377-127">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="fc377-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="fc377-128">Результат сравнения.</span><span class="sxs-lookup"><span data-stu-id="fc377-128">Setting comparison result.</span></span> <span data-ttu-id="fc377-129">Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="fc377-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc377-130">Связи</span><span class="sxs-lookup"><span data-stu-id="fc377-130">Relationships</span></span>
<span data-ttu-id="fc377-131">Нет</span><span class="sxs-lookup"><span data-stu-id="fc377-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc377-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc377-132">JSON Representation</span></span>
<span data-ttu-id="fc377-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc377-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```



