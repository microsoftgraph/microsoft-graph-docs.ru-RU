---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint или в виде вложений в объекты событий и сообщений Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0104b9349427b07ffef570d66b98720155bd7728
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239473"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="3ea54-103">Тип ресурса uploadSession</span><span class="sxs-lookup"><span data-stu-id="3ea54-103">uploadSession resource type</span></span>

<span data-ttu-id="3ea54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ea54-105">Ресурс **uploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для [](message.md) бизнеса или в библиотеки документов SharePoint, а также в элементы событий [и](event.md) сообщений Outlook в виде вложений.</span><span class="sxs-lookup"><span data-stu-id="3ea54-105">The **uploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ea54-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ea54-106">JSON representation</span></span>

<span data-ttu-id="3ea54-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3ea54-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a><span data-ttu-id="3ea54-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ea54-108">Properties</span></span>


| <span data-ttu-id="3ea54-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ea54-109">Property</span></span>       | <span data-ttu-id="3ea54-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ea54-110">Type</span></span>              |<span data-ttu-id="3ea54-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea54-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="3ea54-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea54-112">expirationDateTime</span></span> | <span data-ttu-id="3ea54-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ea54-113">DateTimeOffset</span></span>    | <span data-ttu-id="3ea54-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="3ea54-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="3ea54-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="3ea54-116">nextExpectedRanges</span></span> | <span data-ttu-id="3ea54-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3ea54-117">String collection</span></span> | <span data-ttu-id="3ea54-118">Коллекция диапазонов байтов файла, отсутствующих на сервере.</span><span class="sxs-lookup"><span data-stu-id="3ea54-118">A collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="3ea54-119">Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="3ea54-119">These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="3ea54-120">При отправке файлов в виде вложений Outlook, а не коллекции диапазонов, это свойство всегда указывает одно значение "{start}", расположение в файле, где должна начаться следующая отправка.</span><span class="sxs-lookup"><span data-stu-id="3ea54-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="3ea54-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="3ea54-121">uploadUrl</span></span>          | <span data-ttu-id="3ea54-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3ea54-122">String</span></span>            | <span data-ttu-id="3ea54-123">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="3ea54-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="3ea54-124">См. также</span><span class="sxs-lookup"><span data-stu-id="3ea54-124">See also</span></span>

- [<span data-ttu-id="3ea54-125">Вложение больших файлов в сообщения и события Outlook в виде вложений </span><span class="sxs-lookup"><span data-stu-id="3ea54-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="3ea54-126">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="3ea54-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

