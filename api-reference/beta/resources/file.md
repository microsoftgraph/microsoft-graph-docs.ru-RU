---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Файл
localization_priority: Normal
ms.openlocfilehash: eac17370a9d54d074014d00d6ac53913e6adabd3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333962"
---
# <a name="file-resource-type"></a><span data-ttu-id="f471a-102">Тип ресурса file</span><span class="sxs-lookup"><span data-stu-id="f471a-102">File resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f471a-103">Ресурс **File** — это единая структура, объединяющая элементы данных, связанные с файлами.</span><span class="sxs-lookup"><span data-stu-id="f471a-103">The **File** resource groups file-related data items into a single structure.</span></span>

<span data-ttu-id="f471a-p101">Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **file**, то этот ресурс представляет файл. Помимо других свойств, у файлов есть связь **content**, которая содержит байтовый поток файла.</span><span class="sxs-lookup"><span data-stu-id="f471a-p101">If a [**DriveItem**](driveitem.md) has a non-null **file** facet, the item represents an file. In addition to other properties, files have a **content** relationship which contains the byte stream of the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f471a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f471a-106">JSON representation</span></span>

<span data-ttu-id="f471a-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f471a-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f471a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f471a-108">Properties</span></span>

| <span data-ttu-id="f471a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f471a-109">Property</span></span> | <span data-ttu-id="f471a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f471a-110">Type</span></span>                    | <span data-ttu-id="f471a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f471a-111">Description</span></span>                                                                                                                                      |
|:---------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f471a-112">hashes</span><span class="sxs-lookup"><span data-stu-id="f471a-112">hashes</span></span>   | [<span data-ttu-id="f471a-113">HashesType</span><span class="sxs-lookup"><span data-stu-id="f471a-113">HashesType</span></span>](hashes.md) | <span data-ttu-id="f471a-p102">Хэши двоичного содержимого файла (если они доступны). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f471a-p102">Hashes of the file's binary content, if available. Read-only.</span></span>                                                                                    |
| <span data-ttu-id="f471a-116">mimeType</span><span class="sxs-lookup"><span data-stu-id="f471a-116">mimeType</span></span> | <span data-ttu-id="f471a-117">string</span><span class="sxs-lookup"><span data-stu-id="f471a-117">string</span></span>                  | <span data-ttu-id="f471a-p103">Тип MIME файла. Он определяется логикой на сервере и может не совпадать со значением, предоставленным при отправке файла. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f471a-p103">The MIME type for the file. This is determined by logic on the server and might not be the value provided when the file was uploaded. Read-only.</span></span> |

## <a name="remarks"></a><span data-ttu-id="f471a-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="f471a-121">Remarks</span></span> 

<span data-ttu-id="f471a-122">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f471a-122">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The file facet describes properties of a file",
  "keywords": "file,item,facet",
  "section": "documentation",
  "tocPath": "Facets/File",
  "suppressions": []
}
-->
