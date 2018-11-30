---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077317"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="8cbbf-102">Тип ресурса DeleteAction</span><span class="sxs-lookup"><span data-stu-id="8cbbf-102">DeleteAction resource type</span></span>

> <span data-ttu-id="8cbbf-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cbbf-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cbbf-105">Наличие ресурса **DeleteAction** в ресурсе [**itemActivity**][activity] указывает, что в результате выполнения действия элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8cbbf-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8cbbf-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8cbbf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cbbf-107">Properties</span></span>

| <span data-ttu-id="8cbbf-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8cbbf-108">Property name</span></span> | <span data-ttu-id="8cbbf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8cbbf-109">Type</span></span>   | <span data-ttu-id="8cbbf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8cbbf-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8cbbf-111">name</span><span class="sxs-lookup"><span data-stu-id="8cbbf-111">name</span></span>          | <span data-ttu-id="8cbbf-112">строка</span><span class="sxs-lookup"><span data-stu-id="8cbbf-112">string</span></span> | <span data-ttu-id="8cbbf-113">Имя элемента, который был удален.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="8cbbf-114">objectType</span><span class="sxs-lookup"><span data-stu-id="8cbbf-114">objectType</span></span>    | <span data-ttu-id="8cbbf-115">string</span><span class="sxs-lookup"><span data-stu-id="8cbbf-115">string</span></span> | <span data-ttu-id="8cbbf-116">`File`или `Folder`, в зависимости от типа удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="8cbbf-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="8cbbf-117">Remarks</span></span>

<span data-ttu-id="8cbbf-118">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8cbbf-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
