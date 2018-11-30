---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: bd0cd6ea5f5ee2225392aa61c2dda9b30e2ffbca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080864"
---
# <a name="file-resource-type"></a><span data-ttu-id="0e0fe-102">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="0e0fe-102">File resource type</span></span>

> <span data-ttu-id="0e0fe-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e0fe-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e0fe-105">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-105">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="0e0fe-p102">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-p102">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e0fe-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e0fe-108">JSON representation</span></span>

<span data-ttu-id="0e0fe-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.file"
}-->

```json
{
  "hashes": {"@odata.type": "microsoft.graph.hashes"},
  "mimeType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0e0fe-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e0fe-110">Properties</span></span>

| <span data-ttu-id="0e0fe-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e0fe-111">Property</span></span> | <span data-ttu-id="0e0fe-112">Тип</span><span class="sxs-lookup"><span data-stu-id="0e0fe-112">Type</span></span>                    | <span data-ttu-id="0e0fe-113">Описание</span><span class="sxs-lookup"><span data-stu-id="0e0fe-113">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0e0fe-114">hashes</span><span class="sxs-lookup"><span data-stu-id="0e0fe-114">hashes</span></span>   | [<span data-ttu-id="0e0fe-115">HashesType</span><span class="sxs-lookup"><span data-stu-id="0e0fe-115">HashesType</span></span>](hashes.md) | <span data-ttu-id="0e0fe-p103">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-p103">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="0e0fe-118">mimeType</span><span class="sxs-lookup"><span data-stu-id="0e0fe-118">mimeType</span></span> | <span data-ttu-id="0e0fe-119">string</span><span class="sxs-lookup"><span data-stu-id="0e0fe-119">string</span></span>                  | <span data-ttu-id="0e0fe-p104">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e0fe-p104">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="0e0fe-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="0e0fe-123">Remarks</span></span> 

<span data-ttu-id="0e0fe-124">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0e0fe-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
