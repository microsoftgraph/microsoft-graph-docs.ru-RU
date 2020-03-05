---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: davidmu1
localization_priority: Normal
doc_type: resourcePageType
ms.prod: azure-ad
ms.openlocfilehash: 751ac6af11b8fdb5709dad816ad2e4c7f2cb53db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519997"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="00d5b-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="00d5b-103">targetResource resource type</span></span>

<span data-ttu-id="00d5b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00d5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00d5b-105">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="00d5b-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="00d5b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="00d5b-106">Properties</span></span>

| <span data-ttu-id="00d5b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="00d5b-107">Property</span></span>     | <span data-ttu-id="00d5b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="00d5b-108">Type</span></span>   |<span data-ttu-id="00d5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00d5b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00d5b-110">id</span><span class="sxs-lookup"><span data-stu-id="00d5b-110">id</span></span>|<span data-ttu-id="00d5b-111">String</span><span class="sxs-lookup"><span data-stu-id="00d5b-111">String</span></span>|<span data-ttu-id="00d5b-112">Указывает уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="00d5b-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="00d5b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="00d5b-113">displayName</span></span>|<span data-ttu-id="00d5b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="00d5b-114">String</span></span>|<span data-ttu-id="00d5b-115">Указывает отображаемое имя, заданное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="00d5b-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="00d5b-116">Обычно указывается при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="00d5b-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="00d5b-117">type</span><span class="sxs-lookup"><span data-stu-id="00d5b-117">type</span></span>|<span data-ttu-id="00d5b-118">String</span><span class="sxs-lookup"><span data-stu-id="00d5b-118">String</span></span>|<span data-ttu-id="00d5b-119">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="00d5b-119">Describes the resource type.</span></span>  <span data-ttu-id="00d5b-120">Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.</span><span class="sxs-lookup"><span data-stu-id="00d5b-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="00d5b-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00d5b-121">userPrincipalName</span></span>|<span data-ttu-id="00d5b-122">String</span><span class="sxs-lookup"><span data-stu-id="00d5b-122">String</span></span>|<span data-ttu-id="00d5b-123">Если \*\*\*\* для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.</span><span class="sxs-lookup"><span data-stu-id="00d5b-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="00d5b-124">groupType</span><span class="sxs-lookup"><span data-stu-id="00d5b-124">groupType</span></span>|<span data-ttu-id="00d5b-125">String</span><span class="sxs-lookup"><span data-stu-id="00d5b-125">String</span></span>|<span data-ttu-id="00d5b-126">Если \*\*\*\* для `Group`параметра Type задано значение, это указывает тип группы.</span><span class="sxs-lookup"><span data-stu-id="00d5b-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="00d5b-127">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="00d5b-127">modifiedProperties</span></span>|<span data-ttu-id="00d5b-128">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="00d5b-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="00d5b-129">Указывает имя, старое значение и новое значение каждого атрибута, который изменился.</span><span class="sxs-lookup"><span data-stu-id="00d5b-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="00d5b-130">Значения свойств зависят от **типа**операции.</span><span class="sxs-lookup"><span data-stu-id="00d5b-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00d5b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00d5b-131">JSON representation</span></span>

<span data-ttu-id="00d5b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00d5b-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String", 
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
