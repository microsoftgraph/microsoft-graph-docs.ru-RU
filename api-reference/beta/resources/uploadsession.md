---
author: JeremyKelley
description: <descrption>
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6b047c8eed22647083da07f2e7722269fb872783
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964233"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="b2e52-102">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="b2e52-102">UploadSession resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2e52-103">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b2e52-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e52-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2e52-104">JSON representation</span></span>

<span data-ttu-id="b2e52-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2e52-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b2e52-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e52-106">Properties</span></span>


| <span data-ttu-id="b2e52-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e52-107">Property</span></span>       | <span data-ttu-id="b2e52-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e52-108">Type</span></span>              |<span data-ttu-id="b2e52-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e52-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="b2e52-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b2e52-110">expirationDateTime</span></span> | <span data-ttu-id="b2e52-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e52-111">DateTimeOffset</span></span>    | <span data-ttu-id="b2e52-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="b2e52-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="b2e52-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="b2e52-114">nextExpectedRanges</span></span> | <span data-ttu-id="b2e52-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b2e52-115">String collection</span></span> | <span data-ttu-id="b2e52-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="b2e52-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="b2e52-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="b2e52-118">uploadUrl</span></span>          | <span data-ttu-id="b2e52-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b2e52-119">String</span></span>            | <span data-ttu-id="b2e52-120">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="b2e52-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="b2e52-121">См. также</span><span class="sxs-lookup"><span data-stu-id="b2e52-121">See also</span></span>

- [<span data-ttu-id="b2e52-122">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="b2e52-122">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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
