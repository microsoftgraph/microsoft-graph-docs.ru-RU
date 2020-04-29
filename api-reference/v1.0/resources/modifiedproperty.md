---
title: Тип ресурса Модифиедпроперти
description: Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 13d377f05650f50f9f87f618ca1c9c07d1da70ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534219"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="9a38e-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="9a38e-103">modifiedProperty resource type</span></span>

<span data-ttu-id="9a38e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a38e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a38e-105">Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.</span><span class="sxs-lookup"><span data-stu-id="9a38e-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="9a38e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a38e-106">Properties</span></span>

| <span data-ttu-id="9a38e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a38e-107">Property</span></span>     | <span data-ttu-id="9a38e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a38e-108">Type</span></span>   |<span data-ttu-id="9a38e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a38e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a38e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9a38e-110">displayName</span></span>|<span data-ttu-id="9a38e-111">String</span><span class="sxs-lookup"><span data-stu-id="9a38e-111">String</span></span>|<span data-ttu-id="9a38e-112">Указывает имя свойства целевого атрибута, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="9a38e-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="9a38e-113">newValue</span><span class="sxs-lookup"><span data-stu-id="9a38e-113">newValue</span></span>|<span data-ttu-id="9a38e-114">String</span><span class="sxs-lookup"><span data-stu-id="9a38e-114">String</span></span>|<span data-ttu-id="9a38e-115">Указывает обновленное значение для правильной работы.</span><span class="sxs-lookup"><span data-stu-id="9a38e-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="9a38e-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="9a38e-116">oldValue</span></span>|<span data-ttu-id="9a38e-117">String</span><span class="sxs-lookup"><span data-stu-id="9a38e-117">String</span></span>|<span data-ttu-id="9a38e-118">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="9a38e-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a38e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a38e-119">JSON representation</span></span>

<span data-ttu-id="9a38e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a38e-120">Here is a JSON representation of the resource.</span></span>

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
