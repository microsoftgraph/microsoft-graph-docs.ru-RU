---
author: JeremyKelley
description: Представляет сведения о итеративном процессе для отправки больших файлов в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в виде вложений файлов в объекты сообщений Outlook.
title: Тип ресурса uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 9bf40360d841c88413cb4f08b603432f86e1d8aa
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621394"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="fdec5-103">Тип ресурса uploadSession</span><span class="sxs-lookup"><span data-stu-id="fdec5-103">uploadSession resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdec5-104">Представляет сведения о итеративном процессе для отправки больших файлов в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в объекты [сообщений](message.md) Outlook в качестве вложений.</span><span class="sxs-lookup"><span data-stu-id="fdec5-104">Represents information for an iterative process to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [message](message.md) objects as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdec5-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdec5-105">JSON representation</span></span>

<span data-ttu-id="fdec5-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fdec5-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="fdec5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdec5-107">Properties</span></span>


| <span data-ttu-id="fdec5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdec5-108">Property</span></span>       | <span data-ttu-id="fdec5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fdec5-109">Type</span></span>              |<span data-ttu-id="fdec5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fdec5-110">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="fdec5-111">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fdec5-111">expirationDateTime</span></span> | <span data-ttu-id="fdec5-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdec5-112">DateTimeOffset</span></span>    | <span data-ttu-id="fdec5-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="fdec5-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="fdec5-115">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="fdec5-115">nextExpectedRanges</span></span> | <span data-ttu-id="fdec5-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fdec5-116">String collection</span></span> | <span data-ttu-id="fdec5-117">При отправке файлов в библиотеки документов это коллекция диапазонов байтов, которые сервер отсутствует для файла.</span><span class="sxs-lookup"><span data-stu-id="fdec5-117">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="fdec5-118">Эти диапазоны обозначаются нулевым индексом и форматом "{Start}-{End}" (например, "0-26", чтобы указать первые 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="fdec5-118">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="fdec5-119">Если вы отправляете файлы в виде вложений в сообщениях Outlook, а не из коллекции диапазонов, это свойство всегда указывает на одно значение "{начало}", расположение в файле, где должна начинаться Следующая загрузка.</span><span class="sxs-lookup"><span data-stu-id="fdec5-119">When uploading files as Outlook message attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="fdec5-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="fdec5-120">uploadUrl</span></span>          | <span data-ttu-id="fdec5-121">Строка</span><span class="sxs-lookup"><span data-stu-id="fdec5-121">String</span></span>            | <span data-ttu-id="fdec5-122">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="fdec5-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="fdec5-123">См. также</span><span class="sxs-lookup"><span data-stu-id="fdec5-123">See also</span></span>

- [<span data-ttu-id="fdec5-124">Присоединение больших файлов к сообщениям Outlook в качестве вложений</span><span class="sxs-lookup"><span data-stu-id="fdec5-124">Attach large files to Outlook messages as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="fdec5-125">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="fdec5-125">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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
