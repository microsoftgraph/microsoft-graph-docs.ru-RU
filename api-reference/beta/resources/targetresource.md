---
title: Сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса объекта targetResource для API Microsoft Graph, который поддерживает действия организации (клиента) по отчетам журнала аудита.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2dc8adea2edf11674d844cee4e5548da96882f7d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137587"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="6fc8f-103">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="6fc8f-103">targetResource resource type</span></span>

<span data-ttu-id="6fc8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fc8f-105">Представляет целевые типы ресурсов, связанные с действиями аудита.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="6fc8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fc8f-106">Properties</span></span>

| <span data-ttu-id="6fc8f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fc8f-107">Property</span></span>     | <span data-ttu-id="6fc8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6fc8f-108">Type</span></span>   |<span data-ttu-id="6fc8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6fc8f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fc8f-110">id</span><span class="sxs-lookup"><span data-stu-id="6fc8f-110">id</span></span>|<span data-ttu-id="6fc8f-111">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc8f-111">String</span></span>|<span data-ttu-id="6fc8f-112">Указывает уникальный ИД ресурса.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="6fc8f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6fc8f-113">displayName</span></span>|<span data-ttu-id="6fc8f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc8f-114">String</span></span>|<span data-ttu-id="6fc8f-115">Указывает видимое имя, определенное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="6fc8f-116">Обычно указывается, когда создается ресурс.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="6fc8f-117">type</span><span class="sxs-lookup"><span data-stu-id="6fc8f-117">type</span></span>|<span data-ttu-id="6fc8f-118">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc8f-118">String</span></span>|<span data-ttu-id="6fc8f-119">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-119">Describes the resource type.</span></span>  <span data-ttu-id="6fc8f-120">Примеры значений: `Application` , `Group` , и `ServicePrincipal` `User` .</span><span class="sxs-lookup"><span data-stu-id="6fc8f-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="6fc8f-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6fc8f-121">userPrincipalName</span></span>|<span data-ttu-id="6fc8f-122">String</span><span class="sxs-lookup"><span data-stu-id="6fc8f-122">String</span></span>|<span data-ttu-id="6fc8f-123">Если **за** установлен тип, это включает имя пользователя, инициа которого было инициировано действие; для `User` других `null` типов.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="6fc8f-124">groupType</span><span class="sxs-lookup"><span data-stu-id="6fc8f-124">groupType</span></span>|<span data-ttu-id="6fc8f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6fc8f-125">String</span></span>|<span data-ttu-id="6fc8f-126">Если **за** установлен `Group` тип, это указывает на тип группы.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="6fc8f-127">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="6fc8f-127">modifiedProperties</span></span>|<span data-ttu-id="6fc8f-128">[Коллекция modifiedProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="6fc8f-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="6fc8f-129">Указывает имя, старое значение и новое значение каждого из измененных атрибутов.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="6fc8f-130">Значения свойств зависят от типа **операции.**</span><span class="sxs-lookup"><span data-stu-id="6fc8f-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc8f-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6fc8f-131">JSON representation</span></span>

<span data-ttu-id="6fc8f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fc8f-132">Here is a JSON representation of the resource.</span></span>

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


