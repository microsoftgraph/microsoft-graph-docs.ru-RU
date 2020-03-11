---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint, а также в виде вложений файлов в события и объекты сообщений Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b2540c1abdd5e40ea960dc3672ab7cc788e08ddd
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590015"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="5cd26-103">Тип ресурса uploadSession</span><span class="sxs-lookup"><span data-stu-id="5cd26-103">uploadSession resource type</span></span>

<span data-ttu-id="5cd26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd26-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5cd26-105">Ресурс **uploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, Onedrive для бизнеса или библиотеки документов SharePoint, а также [события](event.md) и элементы [сообщений](message.md) Outlook в качестве вложений.</span><span class="sxs-lookup"><span data-stu-id="5cd26-105">The **uploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cd26-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cd26-106">JSON representation</span></span>

<span data-ttu-id="5cd26-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5cd26-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="5cd26-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cd26-108">Properties</span></span>


| <span data-ttu-id="5cd26-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cd26-109">Property</span></span>       | <span data-ttu-id="5cd26-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5cd26-110">Type</span></span>              |<span data-ttu-id="5cd26-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5cd26-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="5cd26-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cd26-112">expirationDateTime</span></span> | <span data-ttu-id="5cd26-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cd26-113">DateTimeOffset</span></span>    | <span data-ttu-id="5cd26-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="5cd26-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="5cd26-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="5cd26-116">nextExpectedRanges</span></span> | <span data-ttu-id="5cd26-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5cd26-117">String collection</span></span> | <span data-ttu-id="5cd26-118">Коллекция диапазонов байтов файла, отсутствующих на сервере.</span><span class="sxs-lookup"><span data-stu-id="5cd26-118">A collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="5cd26-119">Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="5cd26-119">These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="5cd26-120">При отправке файлов в виде вложений Outlook вместо коллекции диапазонов это свойство всегда указывает на одно значение "{Start}", расположение в файле, в котором должна начаться следующая загрузка.</span><span class="sxs-lookup"><span data-stu-id="5cd26-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="5cd26-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="5cd26-121">uploadUrl</span></span>          | <span data-ttu-id="5cd26-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5cd26-122">String</span></span>            | <span data-ttu-id="5cd26-123">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="5cd26-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="5cd26-124">См. также</span><span class="sxs-lookup"><span data-stu-id="5cd26-124">See also</span></span>

- [<span data-ttu-id="5cd26-125">Присоединение больших файлов к сообщениям и событиям Outlook в качестве вложений</span><span class="sxs-lookup"><span data-stu-id="5cd26-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="5cd26-126">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="5cd26-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
