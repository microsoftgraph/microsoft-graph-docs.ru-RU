---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: davidmu1
localization_priority: Normal
doc_type: resourcePageType
ms.prod: azure-ad
ms.openlocfilehash: a67cfbccf9d05872ec0d9207ac54c51cda222053
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964580"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="ad38a-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="ad38a-103">targetResource resource type</span></span>

<span data-ttu-id="ad38a-104">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="ad38a-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="ad38a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad38a-105">Properties</span></span>

| <span data-ttu-id="ad38a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad38a-106">Property</span></span>     | <span data-ttu-id="ad38a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ad38a-107">Type</span></span>   |<span data-ttu-id="ad38a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ad38a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad38a-109">id</span><span class="sxs-lookup"><span data-stu-id="ad38a-109">id</span></span>|<span data-ttu-id="ad38a-110">String</span><span class="sxs-lookup"><span data-stu-id="ad38a-110">String</span></span>|<span data-ttu-id="ad38a-111">Указывает уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad38a-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="ad38a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ad38a-112">displayName</span></span>|<span data-ttu-id="ad38a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ad38a-113">String</span></span>|<span data-ttu-id="ad38a-114">Указывает отображаемое имя, заданное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad38a-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="ad38a-115">Обычно указывается при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad38a-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="ad38a-116">type</span><span class="sxs-lookup"><span data-stu-id="ad38a-116">type</span></span>|<span data-ttu-id="ad38a-117">String</span><span class="sxs-lookup"><span data-stu-id="ad38a-117">String</span></span>|<span data-ttu-id="ad38a-118">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad38a-118">Describes the resource type.</span></span>  <span data-ttu-id="ad38a-119">Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.</span><span class="sxs-lookup"><span data-stu-id="ad38a-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="ad38a-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad38a-120">userPrincipalName</span></span>|<span data-ttu-id="ad38a-121">String</span><span class="sxs-lookup"><span data-stu-id="ad38a-121">String</span></span>|<span data-ttu-id="ad38a-122">Если \*\*\*\* для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.</span><span class="sxs-lookup"><span data-stu-id="ad38a-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="ad38a-123">groupType</span><span class="sxs-lookup"><span data-stu-id="ad38a-123">groupType</span></span>|<span data-ttu-id="ad38a-124">String</span><span class="sxs-lookup"><span data-stu-id="ad38a-124">String</span></span>|<span data-ttu-id="ad38a-125">Если \*\*\*\* для `Group`параметра Type задано значение, это указывает тип группы.</span><span class="sxs-lookup"><span data-stu-id="ad38a-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="ad38a-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="ad38a-126">modifiedProperties</span></span>|<span data-ttu-id="ad38a-127">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ad38a-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="ad38a-128">Указывает имя, старое значение и новое значение каждого атрибута, который изменился.</span><span class="sxs-lookup"><span data-stu-id="ad38a-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="ad38a-129">Значения свойств зависят от **типа**операции.</span><span class="sxs-lookup"><span data-stu-id="ad38a-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad38a-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad38a-130">JSON representation</span></span>

<span data-ttu-id="ad38a-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad38a-131">Here is a JSON representation of the resource.</span></span>

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
