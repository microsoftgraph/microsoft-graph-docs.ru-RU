---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844458"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="6e321-103">Тип ресурса modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="6e321-103">modifiedProperty resource type</span></span>
<span data-ttu-id="6e321-104">Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить</span><span class="sxs-lookup"><span data-stu-id="6e321-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="6e321-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e321-105">Properties</span></span>
| <span data-ttu-id="6e321-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e321-106">Property</span></span>     | <span data-ttu-id="6e321-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6e321-107">Type</span></span>   |<span data-ttu-id="6e321-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6e321-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e321-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6e321-109">displayName</span></span>|<span data-ttu-id="6e321-110">Строка</span><span class="sxs-lookup"><span data-stu-id="6e321-110">String</span></span>|<span data-ttu-id="6e321-111">Указывает имя свойства для целевой атрибут, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="6e321-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="6e321-112">newValue</span><span class="sxs-lookup"><span data-stu-id="6e321-112">newValue</span></span>|<span data-ttu-id="6e321-113">String</span><span class="sxs-lookup"><span data-stu-id="6e321-113">String</span></span>|<span data-ttu-id="6e321-114">Указывает обновленное значение для свойство.</span><span class="sxs-lookup"><span data-stu-id="6e321-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="6e321-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="6e321-115">oldValue</span></span>|<span data-ttu-id="6e321-116">String</span><span class="sxs-lookup"><span data-stu-id="6e321-116">String</span></span>|<span data-ttu-id="6e321-117">Указывает предыдущее (до обновления) для свойства.</span><span class="sxs-lookup"><span data-stu-id="6e321-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e321-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e321-118">JSON representation</span></span>

<span data-ttu-id="6e321-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e321-119">Here is a JSON representation of the resource.</span></span>

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
