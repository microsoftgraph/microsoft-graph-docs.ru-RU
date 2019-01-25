---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: c5d15c380908f09ef292b7c5794046bad6e95ac8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507952"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="9f4b2-102">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="9f4b2-102">UploadSession resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f4b2-103">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9f4b2-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f4b2-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f4b2-104">JSON representation</span></span>

<span data-ttu-id="9f4b2-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9f4b2-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="9f4b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f4b2-106">Properties</span></span>


| <span data-ttu-id="9f4b2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f4b2-107">Property</span></span>       | <span data-ttu-id="9f4b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f4b2-108">Type</span></span>              |<span data-ttu-id="9f4b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4b2-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="9f4b2-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4b2-110">expirationDateTime</span></span> | <span data-ttu-id="9f4b2-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4b2-111">DateTimeOffset</span></span>    | <span data-ttu-id="9f4b2-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="9f4b2-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="9f4b2-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="9f4b2-114">nextExpectedRanges</span></span> | <span data-ttu-id="9f4b2-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f4b2-115">String collection</span></span> | <span data-ttu-id="9f4b2-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="9f4b2-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="9f4b2-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="9f4b2-118">uploadUrl</span></span>          | <span data-ttu-id="9f4b2-119">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4b2-119">String</span></span>            | <span data-ttu-id="9f4b2-120">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="9f4b2-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="9f4b2-121">См. также</span><span class="sxs-lookup"><span data-stu-id="9f4b2-121">See also</span></span>

- <span data-ttu-id="9f4b2-122">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="9f4b2-122">[Upload large files with an upload session](../api/driveitem-createuploadsession.md)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": [
    "Error: /api-reference/beta/resources/uploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
