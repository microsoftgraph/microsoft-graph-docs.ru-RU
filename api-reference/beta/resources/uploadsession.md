---
author: JeremyKelley
description: Представляет сведения о итеративном процессе для отправки больших файлов в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в виде вложений файлов в события и объекты сообщений Outlook.
title: Тип ресурса uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 64c907559337a1e6c5f40e046726c747751aaf03
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723723"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="6a1ee-103">Тип ресурса uploadSession</span><span class="sxs-lookup"><span data-stu-id="6a1ee-103">uploadSession resource type</span></span>

<span data-ttu-id="6a1ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a1ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a1ee-105">Представляет сведения о итеративном процессе для отправки больших файлов в:</span><span class="sxs-lookup"><span data-stu-id="6a1ee-105">Represents information for an iterative process to upload large files to:</span></span>

- <span data-ttu-id="6a1ee-106">OneDrive</span><span class="sxs-lookup"><span data-stu-id="6a1ee-106">OneDrive</span></span>
- <span data-ttu-id="6a1ee-107">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="6a1ee-107">OneDrive for Business</span></span>
- <span data-ttu-id="6a1ee-108">Библиотеки документов SharePoint</span><span class="sxs-lookup"><span data-stu-id="6a1ee-108">SharePoint document libraries</span></span>
- <span data-ttu-id="6a1ee-109">[События](event.md) и элементы [сообщений](message.md) Outlook в виде вложений</span><span class="sxs-lookup"><span data-stu-id="6a1ee-109">Outlook [event](event.md) and [message](message.md) items as attachments</span></span>
- <span data-ttu-id="6a1ee-110">Элементы универсального принтера [printDocument](printdocument.md)</span><span class="sxs-lookup"><span data-stu-id="6a1ee-110">Universal Print [printDocument](printdocument.md) items</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a1ee-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a1ee-111">JSON representation</span></span>

<span data-ttu-id="6a1ee-112">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-112">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="6a1ee-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a1ee-113">Properties</span></span>


| <span data-ttu-id="6a1ee-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a1ee-114">Property</span></span>       | <span data-ttu-id="6a1ee-115">Тип</span><span class="sxs-lookup"><span data-stu-id="6a1ee-115">Type</span></span>              |<span data-ttu-id="6a1ee-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6a1ee-116">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="6a1ee-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a1ee-117">expirationDateTime</span></span> | <span data-ttu-id="6a1ee-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a1ee-118">DateTimeOffset</span></span>    | <span data-ttu-id="6a1ee-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="6a1ee-121">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="6a1ee-121">nextExpectedRanges</span></span> | <span data-ttu-id="6a1ee-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6a1ee-122">String collection</span></span> | <span data-ttu-id="6a1ee-123">При отправке файлов в библиотеки документов это коллекция диапазонов байтов, которые сервер отсутствует для файла.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-123">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="6a1ee-124">Эти диапазоны обозначаются нулевым индексом и форматом "{Start}-{End}" (например, "0-26", чтобы указать первые 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="6a1ee-124">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="6a1ee-125">При отправке файлов в виде вложений Outlook вместо коллекции диапазонов это свойство всегда указывает на одно значение "{Start}", расположение в файле, в котором должна начаться следующая загрузка.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-125">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="6a1ee-126">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="6a1ee-126">uploadUrl</span></span>          | <span data-ttu-id="6a1ee-127">Строка</span><span class="sxs-lookup"><span data-stu-id="6a1ee-127">String</span></span>            | <span data-ttu-id="6a1ee-128">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-128">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="6a1ee-129">См. также</span><span class="sxs-lookup"><span data-stu-id="6a1ee-129">See also</span></span>

- [<span data-ttu-id="6a1ee-130">Присоединение больших файлов к сообщениям и событиям Outlook в качестве вложений </span><span class="sxs-lookup"><span data-stu-id="6a1ee-130">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="6a1ee-131">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="6a1ee-131">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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


