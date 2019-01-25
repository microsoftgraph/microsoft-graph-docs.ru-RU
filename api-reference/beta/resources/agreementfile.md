---
title: Тип ресурса agreementFile
description: Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511431"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="7ef0b-104">Тип ресурса agreementFile</span><span class="sxs-lookup"><span data-stu-id="7ef0b-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ef0b-105">Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7ef0b-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7ef0b-106">Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="7ef0b-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="7ef0b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ef0b-107">Properties</span></span>
| <span data-ttu-id="7ef0b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ef0b-108">Property</span></span>     | <span data-ttu-id="7ef0b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef0b-109">Type</span></span>        | <span data-ttu-id="7ef0b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef0b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ef0b-111">fileData</span><span class="sxs-lookup"><span data-stu-id="7ef0b-111">fileData</span></span>|[<span data-ttu-id="7ef0b-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="7ef0b-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="7ef0b-113">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="7ef0b-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-114">Read-only.</span></span>|
|<span data-ttu-id="7ef0b-115">fileName</span><span class="sxs-lookup"><span data-stu-id="7ef0b-115">fileName</span></span>|<span data-ttu-id="7ef0b-116">String</span><span class="sxs-lookup"><span data-stu-id="7ef0b-116">String</span></span>|<span data-ttu-id="7ef0b-117">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="7ef0b-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="7ef0b-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-118">Read-only.</span></span>|
|<span data-ttu-id="7ef0b-119">id</span><span class="sxs-lookup"><span data-stu-id="7ef0b-119">id</span></span>|<span data-ttu-id="7ef0b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="7ef0b-120">String</span></span>|<span data-ttu-id="7ef0b-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-121">Read-only.</span></span>|
|<span data-ttu-id="7ef0b-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="7ef0b-122">isDefault</span></span>|<span data-ttu-id="7ef0b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ef0b-123">Boolean</span></span>|<span data-ttu-id="7ef0b-124">Указывает, является ли файл соглашения по умолчанию Если ни одна из культур совпадает с клиентом.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="7ef0b-125">Если ни один из файлов помечены как по умолчанию, первый будет рассматриваться как значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="7ef0b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-126">Read-only.</span></span>|
|<span data-ttu-id="7ef0b-127">language</span><span class="sxs-lookup"><span data-stu-id="7ef0b-127">language</span></span>|<span data-ttu-id="7ef0b-128">String</span><span class="sxs-lookup"><span data-stu-id="7ef0b-128">String</span></span>|<span data-ttu-id="7ef0b-129">Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="7ef0b-130">languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="7ef0b-131">Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US).</span><span class="sxs-lookup"><span data-stu-id="7ef0b-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="7ef0b-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ef0b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="7ef0b-133">Relationships</span></span>
<span data-ttu-id="7ef0b-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7ef0b-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ef0b-135">JSON representation</span></span>

<span data-ttu-id="7ef0b-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ef0b-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
