---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e8c886e3464070d0dba8779741ed65681a764de
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364742"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="535f8-103">Тип ресурса Девицеманажементсеттингкомпарисон</span><span class="sxs-lookup"><span data-stu-id="535f8-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="535f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535f8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="535f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535f8-106">Объект, представляющий результат сравнения параметров</span><span class="sxs-lookup"><span data-stu-id="535f8-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="535f8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="535f8-107">Properties</span></span>
|<span data-ttu-id="535f8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="535f8-108">Property</span></span>|<span data-ttu-id="535f8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="535f8-109">Type</span></span>|<span data-ttu-id="535f8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="535f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="535f8-111">id</span><span class="sxs-lookup"><span data-stu-id="535f8-111">id</span></span>|<span data-ttu-id="535f8-112">String</span><span class="sxs-lookup"><span data-stu-id="535f8-112">String</span></span>|<span data-ttu-id="535f8-113">Идентификатор параметра</span><span class="sxs-lookup"><span data-stu-id="535f8-113">The setting ID</span></span>|
|<span data-ttu-id="535f8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="535f8-114">displayName</span></span>|<span data-ttu-id="535f8-115">Строка</span><span class="sxs-lookup"><span data-stu-id="535f8-115">String</span></span>|<span data-ttu-id="535f8-116">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="535f8-116">The setting's display name</span></span>|
|<span data-ttu-id="535f8-117">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="535f8-117">definitionId</span></span>|<span data-ttu-id="535f8-118">String</span><span class="sxs-lookup"><span data-stu-id="535f8-118">String</span></span>|<span data-ttu-id="535f8-119">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="535f8-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="535f8-120">куррентвалуежсон</span><span class="sxs-lookup"><span data-stu-id="535f8-120">currentValueJson</span></span>|<span data-ttu-id="535f8-121">String</span><span class="sxs-lookup"><span data-stu-id="535f8-121">String</span></span>|<span data-ttu-id="535f8-122">Значение параметра шаблона (или) в формате JSON для текущего способа (или)</span><span class="sxs-lookup"><span data-stu-id="535f8-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="535f8-123">неввалуежсон</span><span class="sxs-lookup"><span data-stu-id="535f8-123">newValueJson</span></span>|<span data-ttu-id="535f8-124">String</span><span class="sxs-lookup"><span data-stu-id="535f8-124">String</span></span>|<span data-ttu-id="535f8-125">Представление нового значения параметра шаблона в формате JSON</span><span class="sxs-lookup"><span data-stu-id="535f8-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="535f8-126">компарисонресулт</span><span class="sxs-lookup"><span data-stu-id="535f8-126">comparisonResult</span></span>|[<span data-ttu-id="535f8-127">девицеманажементкомпарисонресулт</span><span class="sxs-lookup"><span data-stu-id="535f8-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="535f8-128">Результат сравнения.</span><span class="sxs-lookup"><span data-stu-id="535f8-128">Setting comparison result.</span></span> <span data-ttu-id="535f8-129">Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="535f8-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="535f8-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="535f8-130">Relationships</span></span>
<span data-ttu-id="535f8-131">Нет</span><span class="sxs-lookup"><span data-stu-id="535f8-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="535f8-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="535f8-132">JSON Representation</span></span>
<span data-ttu-id="535f8-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="535f8-133">Here is a JSON representation of the resource.</span></span>
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



