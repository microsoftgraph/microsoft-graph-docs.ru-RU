---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a845a6609991041f12266cd97e95460f96bf742f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876764"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="5e92b-102">Тип ресурса DeleteAction</span><span class="sxs-lookup"><span data-stu-id="5e92b-102">DeleteAction resource type</span></span>

> <span data-ttu-id="5e92b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e92b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e92b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e92b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e92b-105">Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="5e92b-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5e92b-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5e92b-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5e92b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e92b-107">Properties</span></span>

| <span data-ttu-id="5e92b-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5e92b-108">Property name</span></span> | <span data-ttu-id="5e92b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e92b-109">Type</span></span>   | <span data-ttu-id="5e92b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e92b-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5e92b-111">name</span><span class="sxs-lookup"><span data-stu-id="5e92b-111">name</span></span>          | <span data-ttu-id="5e92b-112">строка</span><span class="sxs-lookup"><span data-stu-id="5e92b-112">string</span></span> | <span data-ttu-id="5e92b-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="5e92b-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="5e92b-114">objectType</span><span class="sxs-lookup"><span data-stu-id="5e92b-114">objectType</span></span>    | <span data-ttu-id="5e92b-115">string</span><span class="sxs-lookup"><span data-stu-id="5e92b-115">string</span></span> | <span data-ttu-id="5e92b-116">`File`или `Folder`, в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="5e92b-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="5e92b-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="5e92b-117">Remarks</span></span>

<span data-ttu-id="5e92b-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5e92b-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
