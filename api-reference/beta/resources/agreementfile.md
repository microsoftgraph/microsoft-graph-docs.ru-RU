---
title: Тип ресурса Агриментфиле
description: Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: e3e5ad1d2006332b5a8388d37176a8d10dcf895c
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2020
ms.locfileid: "49555648"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="6327a-104">Тип ресурса Агриментфиле</span><span class="sxs-lookup"><span data-stu-id="6327a-104">agreementFile resource type</span></span>

<span data-ttu-id="6327a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6327a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6327a-106">Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="6327a-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6327a-107">Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="6327a-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="6327a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6327a-108">Properties</span></span>
| <span data-ttu-id="6327a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6327a-109">Property</span></span>     | <span data-ttu-id="6327a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6327a-110">Type</span></span>        | <span data-ttu-id="6327a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6327a-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6327a-112">fileData</span><span class="sxs-lookup"><span data-stu-id="6327a-112">fileData</span></span>|[<span data-ttu-id="6327a-113">агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="6327a-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="6327a-114">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="6327a-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="6327a-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6327a-115">Read-only.</span></span>|
|<span data-ttu-id="6327a-116">fileName</span><span class="sxs-lookup"><span data-stu-id="6327a-116">fileName</span></span>|<span data-ttu-id="6327a-117">String</span><span class="sxs-lookup"><span data-stu-id="6327a-117">String</span></span>|<span data-ttu-id="6327a-118">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="6327a-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="6327a-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6327a-119">Read-only.</span></span>|
|<span data-ttu-id="6327a-120">id</span><span class="sxs-lookup"><span data-stu-id="6327a-120">id</span></span>|<span data-ttu-id="6327a-121">String</span><span class="sxs-lookup"><span data-stu-id="6327a-121">String</span></span>|<span data-ttu-id="6327a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6327a-122">Read-only.</span></span>|
|<span data-ttu-id="6327a-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="6327a-123">isDefault</span></span>|<span data-ttu-id="6327a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6327a-124">Boolean</span></span>|<span data-ttu-id="6327a-125">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="6327a-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="6327a-126">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6327a-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="6327a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6327a-127">Read-only.</span></span>|
|<span data-ttu-id="6327a-128">language</span><span class="sxs-lookup"><span data-stu-id="6327a-128">language</span></span>|<span data-ttu-id="6327a-129">String</span><span class="sxs-lookup"><span data-stu-id="6327a-129">String</span></span>|<span data-ttu-id="6327a-130">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="6327a-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="6327a-131">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="6327a-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="6327a-132">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="6327a-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="6327a-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6327a-133">Read-only.</span></span>|
|<span data-ttu-id="6327a-134">исмажорверсион</span><span class="sxs-lookup"><span data-stu-id="6327a-134">isMajorVersion</span></span>|<span data-ttu-id="6327a-135">Логический</span><span class="sxs-lookup"><span data-stu-id="6327a-135">Boolean</span></span>|<span data-ttu-id="6327a-136">Указывает, является ли файл соглашения основным обновлением версии.</span><span class="sxs-lookup"><span data-stu-id="6327a-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="6327a-137">Основные обновления версий делают недействительными принятие соглашений на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="6327a-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="6327a-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6327a-138">createdDateTime</span></span>|<span data-ttu-id="6327a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6327a-139">DateTimeOffset</span></span>|<span data-ttu-id="6327a-140">Дата и время создания файла. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6327a-140">The date time representing when the file was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6327a-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="6327a-141">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="6327a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6327a-142">JSON representation</span></span>

<span data-ttu-id="6327a-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6327a-143">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


