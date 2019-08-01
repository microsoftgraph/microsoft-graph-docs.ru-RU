---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в библиотеки документов OneDrive, OneDrive для бизнеса или SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 49453d730e1195c68b1c6245496e9c5530aba720
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033546"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="1375c-103">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="1375c-103">UploadSession resource</span></span>

<span data-ttu-id="1375c-104">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1375c-104">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1375c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1375c-105">JSON representation</span></span>

<span data-ttu-id="1375c-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1375c-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1375c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1375c-107">Properties</span></span>


| <span data-ttu-id="1375c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1375c-108">Property</span></span>       | <span data-ttu-id="1375c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1375c-109">Type</span></span>              |<span data-ttu-id="1375c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1375c-110">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="1375c-111">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1375c-111">expirationDateTime</span></span> | <span data-ttu-id="1375c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1375c-112">DateTimeOffset</span></span>    | <span data-ttu-id="1375c-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="1375c-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="1375c-115">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="1375c-115">nextExpectedRanges</span></span> | <span data-ttu-id="1375c-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1375c-116">String collection</span></span> | <span data-ttu-id="1375c-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="1375c-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="1375c-119">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="1375c-119">uploadUrl</span></span>          | <span data-ttu-id="1375c-120">Строка</span><span class="sxs-lookup"><span data-stu-id="1375c-120">String</span></span>            | <span data-ttu-id="1375c-121">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="1375c-121">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="1375c-122">См. также</span><span class="sxs-lookup"><span data-stu-id="1375c-122">See also</span></span>

- [<span data-ttu-id="1375c-123">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="1375c-123">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
