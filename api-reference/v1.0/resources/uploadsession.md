---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: Ресурс UploadSession предоставляет сведения о том, как отправлять большие файлы в библиотеки документов OneDrive, OneDrive для бизнеса или SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3537a59da65499e67283d8a0640e5392c65edce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446788"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="69b09-103">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="69b09-103">UploadSession resource</span></span>

<span data-ttu-id="69b09-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69b09-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69b09-105">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="69b09-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69b09-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69b09-106">JSON representation</span></span>

<span data-ttu-id="69b09-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="69b09-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="69b09-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="69b09-108">Properties</span></span>


| <span data-ttu-id="69b09-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="69b09-109">Property</span></span>       | <span data-ttu-id="69b09-110">Тип</span><span class="sxs-lookup"><span data-stu-id="69b09-110">Type</span></span>              |<span data-ttu-id="69b09-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69b09-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="69b09-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="69b09-112">expirationDateTime</span></span> | <span data-ttu-id="69b09-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69b09-113">DateTimeOffset</span></span>    | <span data-ttu-id="69b09-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="69b09-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="69b09-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="69b09-116">nextExpectedRanges</span></span> | <span data-ttu-id="69b09-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="69b09-117">String collection</span></span> | <span data-ttu-id="69b09-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="69b09-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="69b09-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="69b09-120">uploadUrl</span></span>          | <span data-ttu-id="69b09-121">Строка</span><span class="sxs-lookup"><span data-stu-id="69b09-121">String</span></span>            | <span data-ttu-id="69b09-122">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="69b09-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="69b09-123">См. также</span><span class="sxs-lookup"><span data-stu-id="69b09-123">See also</span></span>

- [<span data-ttu-id="69b09-124">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="69b09-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
