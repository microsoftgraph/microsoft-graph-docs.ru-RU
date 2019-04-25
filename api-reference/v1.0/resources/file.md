---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Файл
localization_priority: Normal
ms.openlocfilehash: 7478ba064b5193ce7ddcd8685fc571a72d4b0057
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564787"
---
# <a name="file-resource-type"></a><span data-ttu-id="9b596-102">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="9b596-102">File resource type</span></span>

<span data-ttu-id="9b596-103">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="9b596-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="9b596-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="9b596-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b596-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b596-106">JSON representation</span></span>

<span data-ttu-id="9b596-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b596-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9b596-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b596-108">Properties</span></span>

| <span data-ttu-id="9b596-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b596-109">Property</span></span> | <span data-ttu-id="9b596-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9b596-110">Type</span></span>                    | <span data-ttu-id="9b596-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9b596-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9b596-112">hashes</span><span class="sxs-lookup"><span data-stu-id="9b596-112">hashes</span></span>   | [<span data-ttu-id="9b596-113">Hashes</span><span class="sxs-lookup"><span data-stu-id="9b596-113">Hashes</span></span>](hashes.md) | <span data-ttu-id="9b596-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b596-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="9b596-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="9b596-116">mimeType</span></span> | <span data-ttu-id="9b596-117">string</span><span class="sxs-lookup"><span data-stu-id="9b596-117">string</span></span>                  | <span data-ttu-id="9b596-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b596-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9b596-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="9b596-121">Remarks</span></span> 

<span data-ttu-id="9b596-122">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b596-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File"
} -->
