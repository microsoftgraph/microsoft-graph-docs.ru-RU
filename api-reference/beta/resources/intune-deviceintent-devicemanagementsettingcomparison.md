---
title: Тип ресурса Девицеманажементсеттингкомпарисон
description: Объект, представляющий результат сравнения параметров
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0463da79c2cedc78c5546fa86b5891468f7a4c11
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728281"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="6ad5e-103">Тип ресурса Девицеманажементсеттингкомпарисон</span><span class="sxs-lookup"><span data-stu-id="6ad5e-103">deviceManagementSettingComparison resource type</span></span>

<span data-ttu-id="6ad5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ad5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad5e-107">Объект, представляющий результат сравнения параметров</span><span class="sxs-lookup"><span data-stu-id="6ad5e-107">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="6ad5e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ad5e-108">Properties</span></span>
|<span data-ttu-id="6ad5e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ad5e-109">Property</span></span>|<span data-ttu-id="6ad5e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6ad5e-110">Type</span></span>|<span data-ttu-id="6ad5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6ad5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ad5e-112">id</span><span class="sxs-lookup"><span data-stu-id="6ad5e-112">id</span></span>|<span data-ttu-id="6ad5e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad5e-113">String</span></span>|<span data-ttu-id="6ad5e-114">Идентификатор параметра</span><span class="sxs-lookup"><span data-stu-id="6ad5e-114">The setting ID</span></span>|
|<span data-ttu-id="6ad5e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6ad5e-115">displayName</span></span>|<span data-ttu-id="6ad5e-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad5e-116">String</span></span>|<span data-ttu-id="6ad5e-117">Отображаемое имя параметра</span><span class="sxs-lookup"><span data-stu-id="6ad5e-117">The setting's display name</span></span>|
|<span data-ttu-id="6ad5e-118">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="6ad5e-118">definitionId</span></span>|<span data-ttu-id="6ad5e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad5e-119">String</span></span>|<span data-ttu-id="6ad5e-120">Идентификатор определения параметра для этого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-120">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="6ad5e-121">куррентвалуежсон</span><span class="sxs-lookup"><span data-stu-id="6ad5e-121">currentValueJson</span></span>|<span data-ttu-id="6ad5e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad5e-122">String</span></span>|<span data-ttu-id="6ad5e-123">Значение параметра шаблона (или) в формате JSON для текущего способа (или)</span><span class="sxs-lookup"><span data-stu-id="6ad5e-123">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="6ad5e-124">неввалуежсон</span><span class="sxs-lookup"><span data-stu-id="6ad5e-124">newValueJson</span></span>|<span data-ttu-id="6ad5e-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6ad5e-125">String</span></span>|<span data-ttu-id="6ad5e-126">Представление нового значения параметра шаблона в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ad5e-126">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="6ad5e-127">компарисонресулт</span><span class="sxs-lookup"><span data-stu-id="6ad5e-127">comparisonResult</span></span>|[<span data-ttu-id="6ad5e-128">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="6ad5e-128">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="6ad5e-129">Результат сравнения.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-129">Setting comparison result.</span></span> <span data-ttu-id="6ad5e-130">Возможные значения: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-130">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ad5e-131">Связи</span><span class="sxs-lookup"><span data-stu-id="6ad5e-131">Relationships</span></span>
<span data-ttu-id="6ad5e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="6ad5e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ad5e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ad5e-133">JSON Representation</span></span>
<span data-ttu-id="6ad5e-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ad5e-134">Here is a JSON representation of the resource.</span></span>
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





