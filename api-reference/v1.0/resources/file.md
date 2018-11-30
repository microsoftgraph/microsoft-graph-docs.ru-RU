---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: File
ms.openlocfilehash: 2201533457863c3cac6b7a9463f80e37bd5a569a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026208"
---
# <a name="file-resource-type"></a><span data-ttu-id="c8036-102">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="c8036-102">File resource type</span></span>

<span data-ttu-id="c8036-103">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="c8036-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="c8036-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="c8036-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8036-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c8036-106">JSON representation</span></span>

<span data-ttu-id="c8036-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8036-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8036-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8036-108">Properties</span></span>

| <span data-ttu-id="c8036-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8036-109">Property</span></span> | <span data-ttu-id="c8036-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8036-110">Type</span></span>                    | <span data-ttu-id="c8036-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8036-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c8036-112">hashes</span><span class="sxs-lookup"><span data-stu-id="c8036-112">hashes</span></span>   | [<span data-ttu-id="c8036-113">Hashes</span><span class="sxs-lookup"><span data-stu-id="c8036-113">Hashes</span></span>](hashes.md) | <span data-ttu-id="c8036-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8036-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="c8036-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="c8036-116">mimeType</span></span> | <span data-ttu-id="c8036-117">string</span><span class="sxs-lookup"><span data-stu-id="c8036-117">string</span></span>                  | <span data-ttu-id="c8036-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8036-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c8036-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="c8036-121">Remarks</span></span> 

<span data-ttu-id="c8036-122">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c8036-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
