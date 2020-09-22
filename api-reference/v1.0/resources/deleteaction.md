---
author: daspek
ms.author: dspektor
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0bd96e02e822d1b2e1901667cbbea86ca91c8b3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018734"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="2be03-103">Тип ресурса deleteAction</span><span class="sxs-lookup"><span data-stu-id="2be03-103">deleteAction resource type</span></span>

<span data-ttu-id="2be03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2be03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2be03-105">Присутствие ресурса **deleteAction** в [**itemActivity**][activity] указывает на то, что действие удалило элемент.</span><span class="sxs-lookup"><span data-stu-id="2be03-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="2be03-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2be03-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="2be03-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2be03-107">Properties</span></span>

| <span data-ttu-id="2be03-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2be03-108">Property name</span></span> | <span data-ttu-id="2be03-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2be03-109">Type</span></span>   | <span data-ttu-id="2be03-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2be03-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2be03-111">name</span><span class="sxs-lookup"><span data-stu-id="2be03-111">name</span></span>          | <span data-ttu-id="2be03-112">string</span><span class="sxs-lookup"><span data-stu-id="2be03-112">string</span></span> | <span data-ttu-id="2be03-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="2be03-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="2be03-114">objectType</span><span class="sxs-lookup"><span data-stu-id="2be03-114">objectType</span></span>    | <span data-ttu-id="2be03-115">string</span><span class="sxs-lookup"><span data-stu-id="2be03-115">string</span></span> | <span data-ttu-id="2be03-116">`File` или `Folder` , в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="2be03-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2be03-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2be03-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->

