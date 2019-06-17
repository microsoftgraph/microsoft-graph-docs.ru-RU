---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f68ffd08945662fc291fb5489de67967d3cd1cbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002002"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="6b4ed-103">Тип ресурса Девицеманажементсеттингкомпарисон</span><span class="sxs-lookup"><span data-stu-id="6b4ed-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="6b4ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b4ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b4ed-106">Объект, представляющий результат сравнения параметров</span><span class="sxs-lookup"><span data-stu-id="6b4ed-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="6b4ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b4ed-107">Properties</span></span>
|<span data-ttu-id="6b4ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b4ed-108">Property</span></span>|<span data-ttu-id="6b4ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b4ed-109">Type</span></span>|<span data-ttu-id="6b4ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b4ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b4ed-111">id</span><span class="sxs-lookup"><span data-stu-id="6b4ed-111">id</span></span>|<span data-ttu-id="6b4ed-112">String</span><span class="sxs-lookup"><span data-stu-id="6b4ed-112">String</span></span>|<span data-ttu-id="6b4ed-113">Идентификатор параметра</span><span class="sxs-lookup"><span data-stu-id="6b4ed-113">The setting ID</span></span>|
|<span data-ttu-id="6b4ed-114">displayName</span><span class="sxs-lookup"><span data-stu-id="6b4ed-114">displayName</span></span>|<span data-ttu-id="6b4ed-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6b4ed-115">String</span></span>|<span data-ttu-id="6b4ed-116">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="6b4ed-116">The setting's display name</span></span>|
|<span data-ttu-id="6b4ed-117">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="6b4ed-117">definitionId</span></span>|<span data-ttu-id="6b4ed-118">String</span><span class="sxs-lookup"><span data-stu-id="6b4ed-118">String</span></span>|<span data-ttu-id="6b4ed-119">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="6b4ed-120">Куррентвалуежсон</span><span class="sxs-lookup"><span data-stu-id="6b4ed-120">currentValueJson</span></span>|<span data-ttu-id="6b4ed-121">String</span><span class="sxs-lookup"><span data-stu-id="6b4ed-121">String</span></span>|<span data-ttu-id="6b4ed-122">Значение параметра шаблона (или) в формате JSON для текущего способа (или)</span><span class="sxs-lookup"><span data-stu-id="6b4ed-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="6b4ed-123">Неввалуежсон</span><span class="sxs-lookup"><span data-stu-id="6b4ed-123">newValueJson</span></span>|<span data-ttu-id="6b4ed-124">String</span><span class="sxs-lookup"><span data-stu-id="6b4ed-124">String</span></span>|<span data-ttu-id="6b4ed-125">Представление нового значения параметра шаблона в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b4ed-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="6b4ed-126">Компарисонресулт</span><span class="sxs-lookup"><span data-stu-id="6b4ed-126">comparisonResult</span></span>|[<span data-ttu-id="6b4ed-127">Девицеманажементкомпарисонресулт</span><span class="sxs-lookup"><span data-stu-id="6b4ed-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="6b4ed-128">Результат сравнения.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-128">Setting comparison result.</span></span> <span data-ttu-id="6b4ed-129">Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b4ed-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="6b4ed-130">Relationships</span></span>
<span data-ttu-id="6b4ed-131">Нет</span><span class="sxs-lookup"><span data-stu-id="6b4ed-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b4ed-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b4ed-132">JSON Representation</span></span>
<span data-ttu-id="6b4ed-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b4ed-133">Here is a JSON representation of the resource.</span></span>
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





