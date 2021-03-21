---
title: тип сложного типа ресурсов targetResource — API Microsoft Graph
description: Определяет сложный тип API microsoft Graph, который поддерживает деятельность организации (клиента) по отчету о журнале аудита.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 12030bdb5c51e41e821218e3db67c4878a90c53d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954960"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="02f43-103">тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="02f43-103">targetResource resource type</span></span>

<span data-ttu-id="02f43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02f43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02f43-105">Представляет целевые типы ресурсов, связанные с деятельностью аудита.</span><span class="sxs-lookup"><span data-stu-id="02f43-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="02f43-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="02f43-106">Properties</span></span>

| <span data-ttu-id="02f43-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="02f43-107">Property</span></span>     | <span data-ttu-id="02f43-108">Тип</span><span class="sxs-lookup"><span data-stu-id="02f43-108">Type</span></span>   |<span data-ttu-id="02f43-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02f43-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f43-110">id</span><span class="sxs-lookup"><span data-stu-id="02f43-110">id</span></span>|<span data-ttu-id="02f43-111">Строка</span><span class="sxs-lookup"><span data-stu-id="02f43-111">String</span></span>|<span data-ttu-id="02f43-112">Указывает уникальный ID ресурса.</span><span class="sxs-lookup"><span data-stu-id="02f43-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="02f43-113">displayName</span><span class="sxs-lookup"><span data-stu-id="02f43-113">displayName</span></span>|<span data-ttu-id="02f43-114">Строка</span><span class="sxs-lookup"><span data-stu-id="02f43-114">String</span></span>|<span data-ttu-id="02f43-115">Указывает видимое имя, определенное для ресурса.</span><span class="sxs-lookup"><span data-stu-id="02f43-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="02f43-116">Обычно указывается, когда создается ресурс.</span><span class="sxs-lookup"><span data-stu-id="02f43-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="02f43-117">type</span><span class="sxs-lookup"><span data-stu-id="02f43-117">type</span></span>|<span data-ttu-id="02f43-118">Строка</span><span class="sxs-lookup"><span data-stu-id="02f43-118">String</span></span>|<span data-ttu-id="02f43-119">Описывает тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="02f43-119">Describes the resource type.</span></span>  <span data-ttu-id="02f43-120">Примеры значений включают `Application` `Group` , и `ServicePrincipal` `User` .</span><span class="sxs-lookup"><span data-stu-id="02f43-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="02f43-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02f43-121">userPrincipalName</span></span>|<span data-ttu-id="02f43-122">String</span><span class="sxs-lookup"><span data-stu-id="02f43-122">String</span></span>|<span data-ttu-id="02f43-123">При **наборе** типа включается имя пользователя, которое `User` инициировало действие; для других `null` типов.</span><span class="sxs-lookup"><span data-stu-id="02f43-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="02f43-124">groupType</span><span class="sxs-lookup"><span data-stu-id="02f43-124">groupType</span></span>|<span data-ttu-id="02f43-125">groupType</span><span class="sxs-lookup"><span data-stu-id="02f43-125">groupType</span></span>|<span data-ttu-id="02f43-126">При **наборе** типа указывается тип `Group` группы.</span><span class="sxs-lookup"><span data-stu-id="02f43-126">When **type** is set to `Group`, this indicates the group type.</span></span>  <span data-ttu-id="02f43-127">Возможные значения: `unifiedGroups` `azureAD` , и `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="02f43-127">Possible values are: `unifiedGroups`, `azureAD`, and `unknownFutureValue`</span></span>|
|<span data-ttu-id="02f43-128">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="02f43-128">modifiedProperties</span></span>|<span data-ttu-id="02f43-129">[измененная коллекцияProperty](modifiedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="02f43-129">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="02f43-130">Указывает имя, старое значение и новое значение каждого измененного атрибута.</span><span class="sxs-lookup"><span data-stu-id="02f43-130">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="02f43-131">Значения свойств зависят от **типа операции.**</span><span class="sxs-lookup"><span data-stu-id="02f43-131">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02f43-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02f43-132">JSON representation</span></span>

<span data-ttu-id="02f43-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02f43-133">Here is a JSON representation of the resource.</span></span>

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


