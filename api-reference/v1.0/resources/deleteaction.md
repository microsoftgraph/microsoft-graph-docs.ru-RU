---
author: daspek
title: Тип ресурса deleteAction
description: Объект deleteAction предоставляет сведения об удалении элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e78b4369606b0e0e3880fc3bfd13fdec263fcb58
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239634"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="5fc2a-103">Тип ресурса deleteAction</span><span class="sxs-lookup"><span data-stu-id="5fc2a-103">deleteAction resource type</span></span>

<span data-ttu-id="5fc2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc2a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fc2a-105">Наличие ресурса **deleteAction** в [**itemActivity**][activity] указывает, что действие удалило элемент.</span><span class="sxs-lookup"><span data-stu-id="5fc2a-105">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="5fc2a-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5fc2a-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="5fc2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fc2a-107">Properties</span></span>

| <span data-ttu-id="5fc2a-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5fc2a-108">Property name</span></span> | <span data-ttu-id="5fc2a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5fc2a-109">Type</span></span>   | <span data-ttu-id="5fc2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc2a-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5fc2a-111">name</span><span class="sxs-lookup"><span data-stu-id="5fc2a-111">name</span></span>          | <span data-ttu-id="5fc2a-112">string</span><span class="sxs-lookup"><span data-stu-id="5fc2a-112">string</span></span> | <span data-ttu-id="5fc2a-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="5fc2a-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="5fc2a-114">objectType</span><span class="sxs-lookup"><span data-stu-id="5fc2a-114">objectType</span></span>    | <span data-ttu-id="5fc2a-115">string</span><span class="sxs-lookup"><span data-stu-id="5fc2a-115">string</span></span> | <span data-ttu-id="5fc2a-116">`File` или `Folder` , в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="5fc2a-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5fc2a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fc2a-117">JSON representation</span></span>

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

