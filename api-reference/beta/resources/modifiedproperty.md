---
title: Тип ресурса Модифиедпроперти
description: Указывает все измененные свойства со старым значением и новым значением для всех ресурсов в Azure AD, которые были изменены
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506238"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="a0e7d-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="a0e7d-103">modifiedProperty resource type</span></span>
<span data-ttu-id="a0e7d-104">Указывает все измененные свойства со старым значением и новым значением для всех ресурсов в Azure AD, которые были изменены</span><span class="sxs-lookup"><span data-stu-id="a0e7d-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="a0e7d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0e7d-105">Properties</span></span>
| <span data-ttu-id="a0e7d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0e7d-106">Property</span></span>     | <span data-ttu-id="a0e7d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a0e7d-107">Type</span></span>   |<span data-ttu-id="a0e7d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0e7d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0e7d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a0e7d-109">displayName</span></span>|<span data-ttu-id="a0e7d-110">String</span><span class="sxs-lookup"><span data-stu-id="a0e7d-110">String</span></span>|<span data-ttu-id="a0e7d-111">Указывает имя свойства целевого атрибута, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="a0e7d-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="a0e7d-112">newValue</span><span class="sxs-lookup"><span data-stu-id="a0e7d-112">newValue</span></span>|<span data-ttu-id="a0e7d-113">String</span><span class="sxs-lookup"><span data-stu-id="a0e7d-113">String</span></span>|<span data-ttu-id="a0e7d-114">Указывает обновленное значение для правильной работы.</span><span class="sxs-lookup"><span data-stu-id="a0e7d-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="a0e7d-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="a0e7d-115">oldValue</span></span>|<span data-ttu-id="a0e7d-116">String</span><span class="sxs-lookup"><span data-stu-id="a0e7d-116">String</span></span>|<span data-ttu-id="a0e7d-117">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="a0e7d-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0e7d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0e7d-118">JSON representation</span></span>

<span data-ttu-id="a0e7d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0e7d-119">Here is a JSON representation of the resource.</span></span>

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
