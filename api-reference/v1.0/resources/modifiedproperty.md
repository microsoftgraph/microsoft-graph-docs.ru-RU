---
title: Тип ресурса Модифиедпроперти
description: Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036101"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="60a5c-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="60a5c-103">modifiedProperty resource type</span></span>

<span data-ttu-id="60a5c-104">Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.</span><span class="sxs-lookup"><span data-stu-id="60a5c-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="60a5c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="60a5c-105">Properties</span></span>

| <span data-ttu-id="60a5c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="60a5c-106">Property</span></span>     | <span data-ttu-id="60a5c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="60a5c-107">Type</span></span>   |<span data-ttu-id="60a5c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="60a5c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a5c-109">displayName</span><span class="sxs-lookup"><span data-stu-id="60a5c-109">displayName</span></span>|<span data-ttu-id="60a5c-110">String</span><span class="sxs-lookup"><span data-stu-id="60a5c-110">String</span></span>|<span data-ttu-id="60a5c-111">Указывает имя свойства целевого атрибута, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="60a5c-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="60a5c-112">newValue</span><span class="sxs-lookup"><span data-stu-id="60a5c-112">newValue</span></span>|<span data-ttu-id="60a5c-113">String</span><span class="sxs-lookup"><span data-stu-id="60a5c-113">String</span></span>|<span data-ttu-id="60a5c-114">Указывает обновленное значение для правильной работы.</span><span class="sxs-lookup"><span data-stu-id="60a5c-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="60a5c-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="60a5c-115">oldValue</span></span>|<span data-ttu-id="60a5c-116">String</span><span class="sxs-lookup"><span data-stu-id="60a5c-116">String</span></span>|<span data-ttu-id="60a5c-117">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="60a5c-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60a5c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60a5c-118">JSON representation</span></span>

<span data-ttu-id="60a5c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60a5c-119">Here is a JSON representation of the resource.</span></span>

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
