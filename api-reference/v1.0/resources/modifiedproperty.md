---
title: Тип ресурса Модифиедпроперти
description: Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: d98d0aaa4850e8ef2b82f9f5deb17424c3ab98d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967382"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="ac0cb-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="ac0cb-103">modifiedProperty resource type</span></span>

<span data-ttu-id="ac0cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac0cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac0cb-105">Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.</span><span class="sxs-lookup"><span data-stu-id="ac0cb-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="ac0cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac0cb-106">Properties</span></span>

| <span data-ttu-id="ac0cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac0cb-107">Property</span></span>     | <span data-ttu-id="ac0cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ac0cb-108">Type</span></span>   |<span data-ttu-id="ac0cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0cb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac0cb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ac0cb-110">displayName</span></span>|<span data-ttu-id="ac0cb-111">String</span><span class="sxs-lookup"><span data-stu-id="ac0cb-111">String</span></span>|<span data-ttu-id="ac0cb-112">Указывает имя свойства целевого атрибута, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="ac0cb-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="ac0cb-113">newValue</span><span class="sxs-lookup"><span data-stu-id="ac0cb-113">newValue</span></span>|<span data-ttu-id="ac0cb-114">String</span><span class="sxs-lookup"><span data-stu-id="ac0cb-114">String</span></span>|<span data-ttu-id="ac0cb-115">Указывает обновленное значение для правильной работы.</span><span class="sxs-lookup"><span data-stu-id="ac0cb-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="ac0cb-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="ac0cb-116">oldValue</span></span>|<span data-ttu-id="ac0cb-117">String</span><span class="sxs-lookup"><span data-stu-id="ac0cb-117">String</span></span>|<span data-ttu-id="ac0cb-118">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="ac0cb-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac0cb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac0cb-119">JSON representation</span></span>

<span data-ttu-id="ac0cb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac0cb-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

