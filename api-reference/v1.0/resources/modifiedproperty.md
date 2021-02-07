---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства ресурса Azure AD, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4e34501f5011310eb7ade73d1c5d938cb58e65cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136040"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="159b8-103">Тип ресурса modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="159b8-103">modifiedProperty resource type</span></span>

<span data-ttu-id="159b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="159b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="159b8-105">Указывает все измененные свойства ресурса Azure AD, включая старые и новые значения.</span><span class="sxs-lookup"><span data-stu-id="159b8-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="159b8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="159b8-106">Properties</span></span>

| <span data-ttu-id="159b8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="159b8-107">Property</span></span>     | <span data-ttu-id="159b8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="159b8-108">Type</span></span>   |<span data-ttu-id="159b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="159b8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="159b8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="159b8-110">displayName</span></span>|<span data-ttu-id="159b8-111">String</span><span class="sxs-lookup"><span data-stu-id="159b8-111">String</span></span>|<span data-ttu-id="159b8-112">Указывает имя свойства целевого атрибута, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="159b8-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="159b8-113">newValue</span><span class="sxs-lookup"><span data-stu-id="159b8-113">newValue</span></span>|<span data-ttu-id="159b8-114">String</span><span class="sxs-lookup"><span data-stu-id="159b8-114">String</span></span>|<span data-ttu-id="159b8-115">Указывает обновленное значение для правильности.</span><span class="sxs-lookup"><span data-stu-id="159b8-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="159b8-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="159b8-116">oldValue</span></span>|<span data-ttu-id="159b8-117">String</span><span class="sxs-lookup"><span data-stu-id="159b8-117">String</span></span>|<span data-ttu-id="159b8-118">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="159b8-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="159b8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="159b8-119">JSON representation</span></span>

<span data-ttu-id="159b8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="159b8-120">Here is a JSON representation of the resource.</span></span>

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

