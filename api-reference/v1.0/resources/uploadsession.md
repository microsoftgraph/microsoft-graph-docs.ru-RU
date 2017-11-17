---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: d84b588c28791ab8f1cf6cef1be6af767fa18e47
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="uploadsession-resource"></a><span data-ttu-id="76054-102">Ресурс UploadSession</span><span class="sxs-lookup"><span data-stu-id="76054-102">UploadSession resource</span></span>

<span data-ttu-id="76054-103">Ресурс **UploadSession** предоставляет сведения о том, как отправлять большие файлы в OneDrive, OneDrive для бизнеса или библиотеки документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="76054-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76054-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76054-104">JSON representation</span></span>

<span data-ttu-id="76054-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="76054-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="76054-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="76054-106">Properties</span></span>


| <span data-ttu-id="76054-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="76054-107">Property</span></span>       | <span data-ttu-id="76054-108">Тип</span><span class="sxs-lookup"><span data-stu-id="76054-108">Type</span></span>              |<span data-ttu-id="76054-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76054-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="76054-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="76054-110">expirationDateTime</span></span> | <span data-ttu-id="76054-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76054-111">DateTimeOffset</span></span>    | <span data-ttu-id="76054-p101">Дата и время (в формате UTC) истечения срока действия сеанса. Полный файл необходимо отправить до наступления этого момента.</span><span class="sxs-lookup"><span data-stu-id="76054-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="76054-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="76054-114">nextExpectedRanges</span></span> | <span data-ttu-id="76054-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="76054-115">String collection</span></span> | <span data-ttu-id="76054-p102">Коллекция диапазонов байтов файла, отсутствующих на сервере. Эти диапазоны имеют нулевую индексацию и формат "начало-конец" (например, "0–26" для указания первых 27 байтов файла).</span><span class="sxs-lookup"><span data-stu-id="76054-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="76054-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="76054-118">uploadUrl</span></span>          | <span data-ttu-id="76054-119">Строка</span><span class="sxs-lookup"><span data-stu-id="76054-119">String</span></span>            | <span data-ttu-id="76054-120">URL-адрес конечной точки, принимающей запросы PUT для диапазонов байтов файла.</span><span class="sxs-lookup"><span data-stu-id="76054-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="76054-121">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="76054-121">Additional Resources</span></span>

<span data-ttu-id="76054-122">Сведения о том, как отправлять файлы с помощью сеанса отправки, см. в статье [Отправка больших файлов с помощью сеанса отправки](../api/driveitem_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="76054-122">See [Upload large files with an upload session](../api/driveitem_createuploadsession.md) for details on how to upload files using an upload session.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
