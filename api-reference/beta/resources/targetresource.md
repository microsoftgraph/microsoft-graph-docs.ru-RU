---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583111"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="f3e60-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="f3e60-103">targetResource resource type</span></span>

<span data-ttu-id="f3e60-104">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="f3e60-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="f3e60-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3e60-105">Properties</span></span>

| <span data-ttu-id="f3e60-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3e60-106">Property</span></span>     | <span data-ttu-id="f3e60-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f3e60-107">Type</span></span>   |<span data-ttu-id="f3e60-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f3e60-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3e60-109">id</span><span class="sxs-lookup"><span data-stu-id="f3e60-109">id</span></span>|<span data-ttu-id="f3e60-110">Строка</span><span class="sxs-lookup"><span data-stu-id="f3e60-110">String</span></span>|<span data-ttu-id="f3e60-111">Указывает уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3e60-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="f3e60-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f3e60-112">displayName</span></span>|<span data-ttu-id="f3e60-113">String</span><span class="sxs-lookup"><span data-stu-id="f3e60-113">String</span></span>|<span data-ttu-id="f3e60-114">Указывает отображаемое имя, заданное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3e60-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="f3e60-115">Обычно указывается при создании ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3e60-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="f3e60-116">type</span><span class="sxs-lookup"><span data-stu-id="f3e60-116">type</span></span>|<span data-ttu-id="f3e60-117">String</span><span class="sxs-lookup"><span data-stu-id="f3e60-117">String</span></span>|<span data-ttu-id="f3e60-118">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="f3e60-118">Describes the resource type.</span></span>  <span data-ttu-id="f3e60-119">Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.</span><span class="sxs-lookup"><span data-stu-id="f3e60-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="f3e60-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3e60-120">userPrincipalName</span></span>|<span data-ttu-id="f3e60-121">String</span><span class="sxs-lookup"><span data-stu-id="f3e60-121">String</span></span>|<span data-ttu-id="f3e60-122">Если \*\*\*\* для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.</span><span class="sxs-lookup"><span data-stu-id="f3e60-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="f3e60-123">groupType</span><span class="sxs-lookup"><span data-stu-id="f3e60-123">groupType</span></span>|<span data-ttu-id="f3e60-124">String</span><span class="sxs-lookup"><span data-stu-id="f3e60-124">String</span></span>|<span data-ttu-id="f3e60-125">Если \*\*\*\* для `Group`параметра Type задано значение, это указывает тип группы.</span><span class="sxs-lookup"><span data-stu-id="f3e60-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="f3e60-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="f3e60-126">modifiedProperties</span></span>|<span data-ttu-id="f3e60-127">Коллекция [модифиедпроперти](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f3e60-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="f3e60-128">Указывает имя, старое значение и новое значение каждого атрибута, который изменился.</span><span class="sxs-lookup"><span data-stu-id="f3e60-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="f3e60-129">Значения свойств зависят от **типа**операции.</span><span class="sxs-lookup"><span data-stu-id="f3e60-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3e60-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3e60-130">JSON representation</span></span>

<span data-ttu-id="f3e60-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3e60-131">Here is a JSON representation of the resource.</span></span>

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
