---
title: Тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 6c912a1ad9740148cd40429478a018c6af512fdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533578"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="2f612-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="2f612-103">targetResource resource type</span></span>

<span data-ttu-id="2f612-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f612-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f612-105">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="2f612-105">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="2f612-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f612-106">Properties</span></span>

| <span data-ttu-id="2f612-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f612-107">Property</span></span>     | <span data-ttu-id="2f612-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f612-108">Type</span></span>   |<span data-ttu-id="2f612-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f612-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f612-110">id</span><span class="sxs-lookup"><span data-stu-id="2f612-110">id</span></span>|<span data-ttu-id="2f612-111">Строка</span><span class="sxs-lookup"><span data-stu-id="2f612-111">String</span></span>|<span data-ttu-id="2f612-112">Указывает уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f612-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="2f612-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2f612-113">displayName</span></span>|<span data-ttu-id="2f612-114">Строка</span><span class="sxs-lookup"><span data-stu-id="2f612-114">String</span></span>|<span data-ttu-id="2f612-115">Указывает отображаемое имя, заданное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f612-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="2f612-116">Обычно указывается при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f612-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="2f612-117">type</span><span class="sxs-lookup"><span data-stu-id="2f612-117">type</span></span>|<span data-ttu-id="2f612-118">String</span><span class="sxs-lookup"><span data-stu-id="2f612-118">String</span></span>|<span data-ttu-id="2f612-119">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f612-119">Describes the resource type.</span></span>  <span data-ttu-id="2f612-120">Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.</span><span class="sxs-lookup"><span data-stu-id="2f612-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="2f612-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2f612-121">userPrincipalName</span></span>|<span data-ttu-id="2f612-122">String</span><span class="sxs-lookup"><span data-stu-id="2f612-122">String</span></span>|<span data-ttu-id="2f612-123">Если \*\*\*\* для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.</span><span class="sxs-lookup"><span data-stu-id="2f612-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="2f612-124">groupType</span><span class="sxs-lookup"><span data-stu-id="2f612-124">groupType</span></span>|<span data-ttu-id="2f612-125">Строка</span><span class="sxs-lookup"><span data-stu-id="2f612-125">String</span></span>|<span data-ttu-id="2f612-126">Если \*\*\*\* для `Group`параметра Type задано значение, это указывает тип группы.</span><span class="sxs-lookup"><span data-stu-id="2f612-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="2f612-127">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="2f612-127">modifiedProperties</span></span>|<span data-ttu-id="2f612-128">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="2f612-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="2f612-129">Указывает имя, старое значение и новое значение каждого атрибута, который изменился.</span><span class="sxs-lookup"><span data-stu-id="2f612-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="2f612-130">Значения свойств зависят от **типа**операции.</span><span class="sxs-lookup"><span data-stu-id="2f612-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f612-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f612-131">JSON representation</span></span>

<span data-ttu-id="2f612-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f612-132">Here is a JSON representation of the resource.</span></span>

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
