---
title: Тип ресурса Агриментфиле
description: Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535755"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="78e19-104">Тип ресурса Агриментфиле</span><span class="sxs-lookup"><span data-stu-id="78e19-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78e19-105">Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="78e19-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="78e19-106">Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="78e19-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="78e19-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="78e19-107">Properties</span></span>
| <span data-ttu-id="78e19-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="78e19-108">Property</span></span>     | <span data-ttu-id="78e19-109">Тип</span><span class="sxs-lookup"><span data-stu-id="78e19-109">Type</span></span>        | <span data-ttu-id="78e19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="78e19-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78e19-111">fileData</span><span class="sxs-lookup"><span data-stu-id="78e19-111">fileData</span></span>|[<span data-ttu-id="78e19-112">Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="78e19-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="78e19-113">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="78e19-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="78e19-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78e19-114">Read-only.</span></span>|
|<span data-ttu-id="78e19-115">fileName</span><span class="sxs-lookup"><span data-stu-id="78e19-115">fileName</span></span>|<span data-ttu-id="78e19-116">String</span><span class="sxs-lookup"><span data-stu-id="78e19-116">String</span></span>|<span data-ttu-id="78e19-117">Имя файла соглашения (например, Тау. PDF).</span><span class="sxs-lookup"><span data-stu-id="78e19-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="78e19-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78e19-118">Read-only.</span></span>|
|<span data-ttu-id="78e19-119">id</span><span class="sxs-lookup"><span data-stu-id="78e19-119">id</span></span>|<span data-ttu-id="78e19-120">String</span><span class="sxs-lookup"><span data-stu-id="78e19-120">String</span></span>|<span data-ttu-id="78e19-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78e19-121">Read-only.</span></span>|
|<span data-ttu-id="78e19-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="78e19-122">isDefault</span></span>|<span data-ttu-id="78e19-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="78e19-123">Boolean</span></span>|<span data-ttu-id="78e19-124">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="78e19-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="78e19-125">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="78e19-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="78e19-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78e19-126">Read-only.</span></span>|
|<span data-ttu-id="78e19-127">language</span><span class="sxs-lookup"><span data-stu-id="78e19-127">language</span></span>|<span data-ttu-id="78e19-128">String</span><span class="sxs-lookup"><span data-stu-id="78e19-128">String</span></span>|<span data-ttu-id="78e19-129">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="78e19-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="78e19-130">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="78e19-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="78e19-131">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="78e19-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="78e19-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78e19-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78e19-133">Связи</span><span class="sxs-lookup"><span data-stu-id="78e19-133">Relationships</span></span>
<span data-ttu-id="78e19-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78e19-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="78e19-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78e19-135">JSON representation</span></span>

<span data-ttu-id="78e19-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78e19-136">The following is a JSON representation of the resource.</span></span>

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
