---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: 3e97a6396f39db690be8a1cfe235bb21592da4e0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481554"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="87965-102">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="87965-102">UploadSession resource</span></span>

<span data-ttu-id="87965-103">Ресурс **UploadSession** содержит сведения о способе отправки больших файлов в OneDrive, OneDrive для бизнеса или в библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="87965-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87965-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87965-104">JSON representation</span></span>

<span data-ttu-id="87965-105">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87965-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="87965-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87965-106">Properties</span></span>


| <span data-ttu-id="87965-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87965-107">Property</span></span>       | <span data-ttu-id="87965-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87965-108">Type</span></span>              |<span data-ttu-id="87965-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87965-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="87965-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="87965-110">expirationDateTime</span></span> | <span data-ttu-id="87965-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87965-111">DateTimeOffset</span></span>    | <span data-ttu-id="87965-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="87965-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="87965-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="87965-114">nextExpectedRanges</span></span> | <span data-ttu-id="87965-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="87965-115">String collection</span></span> | <span data-ttu-id="87965-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="87965-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="87965-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="87965-118">uploadUrl</span></span>          | <span data-ttu-id="87965-119">Строка</span><span class="sxs-lookup"><span data-stu-id="87965-119">String</span></span>            | <span data-ttu-id="87965-120">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="87965-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="87965-121">См. также</span><span class="sxs-lookup"><span data-stu-id="87965-121">See also</span></span>

- [<span data-ttu-id="87965-122">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="87965-122">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
