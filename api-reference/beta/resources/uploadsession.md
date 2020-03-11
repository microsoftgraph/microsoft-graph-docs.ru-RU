---
author: JeremyKelley
description: Представляет сведения о итеративном процессе для отправки больших файлов в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в виде вложений файлов в события и объекты сообщений Outlook.
title: Тип ресурса uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 5a9c205e2cc4e9c151985f1838f69143fbae79e6
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590965"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="5cf5c-103">Тип ресурса uploadSession</span><span class="sxs-lookup"><span data-stu-id="5cf5c-103">uploadSession resource type</span></span>

<span data-ttu-id="5cf5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cf5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf5c-105">Представляет сведения о итеративном процессе для отправки больших файлов в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также [события](event.md) и элементы [сообщений](message.md) Outlook в качестве вложений.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-105">Represents information for an iterative process to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cf5c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cf5c-106">JSON representation</span></span>

<span data-ttu-id="5cf5c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession",
  "baseType": null
}-->

```json
{
  "uploadUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": ["String"]
}
```

## <a name="properties"></a><span data-ttu-id="5cf5c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cf5c-108">Properties</span></span>


| <span data-ttu-id="5cf5c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cf5c-109">Property</span></span>       | <span data-ttu-id="5cf5c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5cf5c-110">Type</span></span>              |<span data-ttu-id="5cf5c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5cf5c-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="5cf5c-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf5c-112">expirationDateTime</span></span> | <span data-ttu-id="5cf5c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf5c-113">DateTimeOffset</span></span>    | <span data-ttu-id="5cf5c-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="5cf5c-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="5cf5c-116">nextExpectedRanges</span></span> | <span data-ttu-id="5cf5c-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5cf5c-117">String collection</span></span> | <span data-ttu-id="5cf5c-118">При отправке файлов в библиотеки документов это коллекция диапазонов байтов, которые сервер отсутствует для файла.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-118">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="5cf5c-119">Эти диапазоны обозначаются нулевым индексом и форматом "{Start}-{End}" (например, "0-26", чтобы указать первые 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="5cf5c-119">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="5cf5c-120">При отправке файлов в виде вложений Outlook вместо коллекции диапазонов это свойство всегда указывает на одно значение "{Start}", расположение в файле, в котором должна начаться следующая загрузка.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="5cf5c-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="5cf5c-121">uploadUrl</span></span>          | <span data-ttu-id="5cf5c-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5cf5c-122">String</span></span>            | <span data-ttu-id="5cf5c-123">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="5cf5c-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="5cf5c-124">См. также</span><span class="sxs-lookup"><span data-stu-id="5cf5c-124">See also</span></span>

- [<span data-ttu-id="5cf5c-125">Присоединение больших файлов к сообщениям и событиям Outlook в качестве вложений</span><span class="sxs-lookup"><span data-stu-id="5cf5c-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="5cf5c-126">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="5cf5c-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->
