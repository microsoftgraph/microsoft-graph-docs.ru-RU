---
author: daspek
ms.author: dspektor
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4d19b41d886c459822abc2ea1b04acebd94c7b68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531690"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="a4158-103">Тип ресурса deleteAction</span><span class="sxs-lookup"><span data-stu-id="a4158-103">deleteAction resource type</span></span>

<span data-ttu-id="a4158-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4158-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4158-105">Присутствие ресурса **deleteAction** в [**itemActivity**][activity] указывает на то, что действие удалило элемент.</span><span class="sxs-lookup"><span data-stu-id="a4158-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="a4158-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a4158-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="a4158-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4158-107">Properties</span></span>

| <span data-ttu-id="a4158-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a4158-108">Property name</span></span> | <span data-ttu-id="a4158-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a4158-109">Type</span></span>   | <span data-ttu-id="a4158-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4158-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a4158-111">name</span><span class="sxs-lookup"><span data-stu-id="a4158-111">name</span></span>          | <span data-ttu-id="a4158-112">string</span><span class="sxs-lookup"><span data-stu-id="a4158-112">string</span></span> | <span data-ttu-id="a4158-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="a4158-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="a4158-114">objectType</span><span class="sxs-lookup"><span data-stu-id="a4158-114">objectType</span></span>    | <span data-ttu-id="a4158-115">string</span><span class="sxs-lookup"><span data-stu-id="a4158-115">string</span></span> | <span data-ttu-id="a4158-116">`File`или `Folder`, в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="a4158-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a4158-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4158-117">JSON representation</span></span>

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
