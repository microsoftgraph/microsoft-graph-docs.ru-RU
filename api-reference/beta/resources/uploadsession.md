---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: 928dc79ae62b5b8b6f6789e42c719eb832135dcb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847504"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="8df34-102">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="8df34-102">UploadSession resource</span></span>

> <span data-ttu-id="8df34-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8df34-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8df34-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df34-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8df34-105">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8df34-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8df34-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8df34-106">JSON representation</span></span>

<span data-ttu-id="8df34-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8df34-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8df34-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8df34-108">Properties</span></span>


| <span data-ttu-id="8df34-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8df34-109">Property</span></span>       | <span data-ttu-id="8df34-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8df34-110">Type</span></span>              |<span data-ttu-id="8df34-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8df34-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="8df34-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8df34-112">expirationDateTime</span></span> | <span data-ttu-id="8df34-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8df34-113">DateTimeOffset</span></span>    | <span data-ttu-id="8df34-p102">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="8df34-p102">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="8df34-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="8df34-116">nextExpectedRanges</span></span> | <span data-ttu-id="8df34-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8df34-117">String collection</span></span> | <span data-ttu-id="8df34-p103">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="8df34-p103">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="8df34-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="8df34-120">uploadUrl</span></span>          | <span data-ttu-id="8df34-121">Строка</span><span class="sxs-lookup"><span data-stu-id="8df34-121">String</span></span>            | <span data-ttu-id="8df34-122">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="8df34-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="8df34-123">См. также</span><span class="sxs-lookup"><span data-stu-id="8df34-123">See also</span></span>

- [<span data-ttu-id="8df34-124">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="8df34-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
