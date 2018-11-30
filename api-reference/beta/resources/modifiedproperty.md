---
title: Тип ресурса modifiedProperty
description: Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077437"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="80024-103">Тип ресурса modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="80024-103">modifiedProperty resource type</span></span>
<span data-ttu-id="80024-104">Указывает все измененные свойства с старое значение и новое значение для любого ресурса в Azure AD, необходимо изменить</span><span class="sxs-lookup"><span data-stu-id="80024-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="80024-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="80024-105">Properties</span></span>
| <span data-ttu-id="80024-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="80024-106">Property</span></span>     | <span data-ttu-id="80024-107">Тип</span><span class="sxs-lookup"><span data-stu-id="80024-107">Type</span></span>   |<span data-ttu-id="80024-108">Описание</span><span class="sxs-lookup"><span data-stu-id="80024-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80024-109">displayName</span><span class="sxs-lookup"><span data-stu-id="80024-109">displayName</span></span>|<span data-ttu-id="80024-110">String</span><span class="sxs-lookup"><span data-stu-id="80024-110">String</span></span>|<span data-ttu-id="80024-111">Указывает имя свойства для целевой атрибут, который был изменен.</span><span class="sxs-lookup"><span data-stu-id="80024-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="80024-112">newValue</span><span class="sxs-lookup"><span data-stu-id="80024-112">newValue</span></span>|<span data-ttu-id="80024-113">String</span><span class="sxs-lookup"><span data-stu-id="80024-113">String</span></span>|<span data-ttu-id="80024-114">Указывает обновленное значение для свойство.</span><span class="sxs-lookup"><span data-stu-id="80024-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="80024-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="80024-115">oldValue</span></span>|<span data-ttu-id="80024-116">String</span><span class="sxs-lookup"><span data-stu-id="80024-116">String</span></span>|<span data-ttu-id="80024-117">Указывает предыдущее (до обновления) для свойства.</span><span class="sxs-lookup"><span data-stu-id="80024-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80024-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80024-118">JSON representation</span></span>

<span data-ttu-id="80024-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80024-119">Here is a JSON representation of the resource.</span></span>

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