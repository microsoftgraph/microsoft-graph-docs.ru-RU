---
title: Тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: 33a381d6088245be235f37549184183443fe3237
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629217"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="7a90c-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="7a90c-103">targetResource resource type</span></span>

<span data-ttu-id="7a90c-104">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="7a90c-104">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="7a90c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a90c-105">Properties</span></span>

| <span data-ttu-id="7a90c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a90c-106">Property</span></span>     | <span data-ttu-id="7a90c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7a90c-107">Type</span></span>   |<span data-ttu-id="7a90c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7a90c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a90c-109">id</span><span class="sxs-lookup"><span data-stu-id="7a90c-109">id</span></span>|<span data-ttu-id="7a90c-110">String</span><span class="sxs-lookup"><span data-stu-id="7a90c-110">String</span></span>|<span data-ttu-id="7a90c-111">Указывает уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="7a90c-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="7a90c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7a90c-112">displayName</span></span>|<span data-ttu-id="7a90c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="7a90c-113">String</span></span>|<span data-ttu-id="7a90c-114">Указывает отображаемое имя, заданное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="7a90c-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="7a90c-115">Обычно указывается при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="7a90c-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="7a90c-116">type</span><span class="sxs-lookup"><span data-stu-id="7a90c-116">type</span></span>|<span data-ttu-id="7a90c-117">String</span><span class="sxs-lookup"><span data-stu-id="7a90c-117">String</span></span>|<span data-ttu-id="7a90c-118">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="7a90c-118">Describes the resource type.</span></span>  <span data-ttu-id="7a90c-119">Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.</span><span class="sxs-lookup"><span data-stu-id="7a90c-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="7a90c-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a90c-120">userPrincipalName</span></span>|<span data-ttu-id="7a90c-121">String</span><span class="sxs-lookup"><span data-stu-id="7a90c-121">String</span></span>|<span data-ttu-id="7a90c-122">Если \*\*\*\* для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.</span><span class="sxs-lookup"><span data-stu-id="7a90c-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="7a90c-123">groupType</span><span class="sxs-lookup"><span data-stu-id="7a90c-123">groupType</span></span>|<span data-ttu-id="7a90c-124">String</span><span class="sxs-lookup"><span data-stu-id="7a90c-124">String</span></span>|<span data-ttu-id="7a90c-125">Если \*\*\*\* для `Group`параметра Type задано значение, это указывает тип группы.</span><span class="sxs-lookup"><span data-stu-id="7a90c-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="7a90c-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="7a90c-126">modifiedProperties</span></span>|<span data-ttu-id="7a90c-127">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7a90c-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="7a90c-128">Указывает имя, старое значение и новое значение каждого атрибута, который изменился.</span><span class="sxs-lookup"><span data-stu-id="7a90c-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="7a90c-129">Значения свойств зависят от **типа**операции.</span><span class="sxs-lookup"><span data-stu-id="7a90c-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a90c-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a90c-130">JSON representation</span></span>

<span data-ttu-id="7a90c-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a90c-131">Here is a JSON representation of the resource.</span></span>

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
