---
title: параметр типа ресурса
description: Представляет параметр, используемый в базовой линии.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2545dc6aa11668359fa9dda636412d36f8d92de1
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403164"
---
# <a name="setting-resource-type"></a><span data-ttu-id="aa62f-103">параметр типа ресурса</span><span class="sxs-lookup"><span data-stu-id="aa62f-103">setting resource type</span></span>

<span data-ttu-id="aa62f-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="aa62f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa62f-105">Представляет параметр, используемый в базовой линии.</span><span class="sxs-lookup"><span data-stu-id="aa62f-105">Represents a setting that is used within a baseline.</span></span>

## <a name="properties"></a><span data-ttu-id="aa62f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa62f-106">Properties</span></span>
|<span data-ttu-id="aa62f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa62f-107">Property</span></span>|<span data-ttu-id="aa62f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa62f-108">Type</span></span>|<span data-ttu-id="aa62f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa62f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa62f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="aa62f-110">displayName</span></span>|<span data-ttu-id="aa62f-111">String</span><span class="sxs-lookup"><span data-stu-id="aa62f-111">String</span></span>|<span data-ttu-id="aa62f-112">Имя отображения для параметра.</span><span class="sxs-lookup"><span data-stu-id="aa62f-112">The display name for the setting.</span></span> <span data-ttu-id="aa62f-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa62f-113">Required.</span></span> <span data-ttu-id="aa62f-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa62f-114">Read-only.</span></span>|
|<span data-ttu-id="aa62f-115">jsonValue</span><span class="sxs-lookup"><span data-stu-id="aa62f-115">jsonValue</span></span>|<span data-ttu-id="aa62f-116">String</span><span class="sxs-lookup"><span data-stu-id="aa62f-116">String</span></span>|<span data-ttu-id="aa62f-117">Значение для параметра, сериализированного как строка JSON.</span><span class="sxs-lookup"><span data-stu-id="aa62f-117">The value for the setting serialized as string of JSON.</span></span> <span data-ttu-id="aa62f-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa62f-118">Required.</span></span> <span data-ttu-id="aa62f-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa62f-119">Read-only.</span></span>|
|<span data-ttu-id="aa62f-120">overwriteAllowed</span><span class="sxs-lookup"><span data-stu-id="aa62f-120">overwriteAllowed</span></span>|<span data-ttu-id="aa62f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa62f-121">Boolean</span></span>|<span data-ttu-id="aa62f-122">Флаг, указывающий, можно ли переопредить существующие конфигурации при применении.</span><span class="sxs-lookup"><span data-stu-id="aa62f-122">A flag indicating whether the setting can be override existing configurations when applied.</span></span> <span data-ttu-id="aa62f-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa62f-123">Required.</span></span> <span data-ttu-id="aa62f-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa62f-124">Read-only.</span></span>|
|<span data-ttu-id="aa62f-125">valueType</span><span class="sxs-lookup"><span data-stu-id="aa62f-125">valueType</span></span>|<span data-ttu-id="aa62f-126">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="aa62f-126">managementParameterValueType</span></span>|<span data-ttu-id="aa62f-127">Тип данных для параметра.</span><span class="sxs-lookup"><span data-stu-id="aa62f-127">The data type for the setting.</span></span> <span data-ttu-id="aa62f-128">Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aa62f-128">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="aa62f-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa62f-129">Required.</span></span> <span data-ttu-id="aa62f-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa62f-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa62f-131">Связи</span><span class="sxs-lookup"><span data-stu-id="aa62f-131">Relationships</span></span>
<span data-ttu-id="aa62f-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa62f-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa62f-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa62f-133">JSON representation</span></span>
<span data-ttu-id="aa62f-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa62f-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
