---
title: Тип ресурса Модифиедпроперти
description: Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: d87d0170dc811db074026e60efc63df928c65ada
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629280"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="ea792-103">Тип ресурса Модифиедпроперти</span><span class="sxs-lookup"><span data-stu-id="ea792-103">modifiedProperty resource type</span></span>

<span data-ttu-id="ea792-104">Указывает все свойства в ресурсе Azure AD, которые были изменены, включая старые и новые значения.</span><span class="sxs-lookup"><span data-stu-id="ea792-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="ea792-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea792-105">Properties</span></span>

| <span data-ttu-id="ea792-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea792-106">Property</span></span>     | <span data-ttu-id="ea792-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ea792-107">Type</span></span>   |<span data-ttu-id="ea792-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ea792-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea792-109">displayName</span><span class="sxs-lookup"><span data-stu-id="ea792-109">displayName</span></span>|<span data-ttu-id="ea792-110">String</span><span class="sxs-lookup"><span data-stu-id="ea792-110">String</span></span>|<span data-ttu-id="ea792-111">Указывает имя свойства целевого атрибута, которое было изменено.</span><span class="sxs-lookup"><span data-stu-id="ea792-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="ea792-112">newValue</span><span class="sxs-lookup"><span data-stu-id="ea792-112">newValue</span></span>|<span data-ttu-id="ea792-113">String</span><span class="sxs-lookup"><span data-stu-id="ea792-113">String</span></span>|<span data-ttu-id="ea792-114">Указывает обновленное значение для правильной работы.</span><span class="sxs-lookup"><span data-stu-id="ea792-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="ea792-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="ea792-115">oldValue</span></span>|<span data-ttu-id="ea792-116">String</span><span class="sxs-lookup"><span data-stu-id="ea792-116">String</span></span>|<span data-ttu-id="ea792-117">Указывает предыдущее значение свойства (перед обновлением).</span><span class="sxs-lookup"><span data-stu-id="ea792-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea792-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ea792-118">JSON representation</span></span>

<span data-ttu-id="ea792-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea792-119">Here is a JSON representation of the resource.</span></span>

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
