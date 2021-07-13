---
title: тип ресурса templateParameter
description: Представляет параметр, использованный в шаблоне управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403160"
---
# <a name="templateparameter-resource-type"></a><span data-ttu-id="9e3bb-103">тип ресурса templateParameter</span><span class="sxs-lookup"><span data-stu-id="9e3bb-103">templateParameter resource type</span></span>

<span data-ttu-id="9e3bb-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="9e3bb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e3bb-105">Представляет параметр, использованный в шаблоне управления.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-105">Represents a parameter utilized in a management template.</span></span>

## <a name="properties"></a><span data-ttu-id="9e3bb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e3bb-106">Properties</span></span>
|<span data-ttu-id="9e3bb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e3bb-107">Property</span></span>|<span data-ttu-id="9e3bb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9e3bb-108">Type</span></span>|<span data-ttu-id="9e3bb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e3bb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e3bb-110">description</span><span class="sxs-lookup"><span data-stu-id="9e3bb-110">description</span></span>|<span data-ttu-id="9e3bb-111">String</span><span class="sxs-lookup"><span data-stu-id="9e3bb-111">String</span></span>|<span data-ttu-id="9e3bb-112">Описание параметра шаблона.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-112">The description for the template parameter.</span></span> <span data-ttu-id="9e3bb-113">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-113">Optional.</span></span> <span data-ttu-id="9e3bb-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-114">Read-only.</span></span>|
|<span data-ttu-id="9e3bb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9e3bb-115">displayName</span></span>|<span data-ttu-id="9e3bb-116">String</span><span class="sxs-lookup"><span data-stu-id="9e3bb-116">String</span></span>|<span data-ttu-id="9e3bb-117">Имя отображения параметра шаблона.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-117">The display name for the template parameter.</span></span> <span data-ttu-id="9e3bb-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-118">Required.</span></span> <span data-ttu-id="9e3bb-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-119">Read-only.</span></span>|
|<span data-ttu-id="9e3bb-120">jsonAllowedValues</span><span class="sxs-lookup"><span data-stu-id="9e3bb-120">jsonAllowedValues</span></span>|<span data-ttu-id="9e3bb-121">String</span><span class="sxs-lookup"><span data-stu-id="9e3bb-121">String</span></span>|<span data-ttu-id="9e3bb-122">Допустимые значения параметра шаблона, представленные сериализированной строкой JSON.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-122">The allowed values for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="9e3bb-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-123">Optional.</span></span> <span data-ttu-id="9e3bb-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-124">Read-only.</span></span>|
|<span data-ttu-id="9e3bb-125">jsonDefaultValue</span><span class="sxs-lookup"><span data-stu-id="9e3bb-125">jsonDefaultValue</span></span>|<span data-ttu-id="9e3bb-126">String</span><span class="sxs-lookup"><span data-stu-id="9e3bb-126">String</span></span>|<span data-ttu-id="9e3bb-127">Значение по умолчанию для параметра шаблона, представленное последовательной строкой JSON.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-127">The default value for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="9e3bb-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-128">Required.</span></span> <span data-ttu-id="9e3bb-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-129">Read-only.</span></span>|
|<span data-ttu-id="9e3bb-130">valueType</span><span class="sxs-lookup"><span data-stu-id="9e3bb-130">valueType</span></span>|<span data-ttu-id="9e3bb-131">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="9e3bb-131">managementParameterValueType</span></span>|<span data-ttu-id="9e3bb-132">Тип данных для параметра шаблона..</span><span class="sxs-lookup"><span data-stu-id="9e3bb-132">The data type for the template parameter..</span></span> <span data-ttu-id="9e3bb-133">Возможные значения: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-133">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="9e3bb-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-134">Required.</span></span> <span data-ttu-id="9e3bb-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e3bb-136">Связи</span><span class="sxs-lookup"><span data-stu-id="9e3bb-136">Relationships</span></span>
<span data-ttu-id="9e3bb-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e3bb-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e3bb-138">JSON representation</span></span>
<span data-ttu-id="9e3bb-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e3bb-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
