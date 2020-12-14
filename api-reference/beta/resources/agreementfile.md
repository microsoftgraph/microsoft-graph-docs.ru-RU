---
title: Тип ресурса agreementFile
description: Представляет настраиваемый файл соглашений об условиях использования, управляемый клиентом с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык и то, является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 12c45876558a162b910120e62c6997c251f391e1
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664026"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="16cf4-104">Тип ресурса agreementFile</span><span class="sxs-lookup"><span data-stu-id="16cf4-104">agreementFile resource type</span></span>

<span data-ttu-id="16cf4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16cf4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16cf4-106">Представляет настраиваемый файл соглашения об условиях использования, управляемый клиентом с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="16cf4-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="16cf4-107">Содержит метаданные о файле соглашения (например, имя, язык и то, является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="16cf4-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="16cf4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="16cf4-108">Properties</span></span>
| <span data-ttu-id="16cf4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="16cf4-109">Property</span></span>     | <span data-ttu-id="16cf4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="16cf4-110">Type</span></span>        | <span data-ttu-id="16cf4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16cf4-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16cf4-112">fileData</span><span class="sxs-lookup"><span data-stu-id="16cf4-112">fileData</span></span>|[<span data-ttu-id="16cf4-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="16cf4-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="16cf4-114">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="16cf4-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="16cf4-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cf4-115">Read-only.</span></span>|
|<span data-ttu-id="16cf4-116">fileName</span><span class="sxs-lookup"><span data-stu-id="16cf4-116">fileName</span></span>|<span data-ttu-id="16cf4-117">String</span><span class="sxs-lookup"><span data-stu-id="16cf4-117">String</span></span>|<span data-ttu-id="16cf4-118">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="16cf4-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="16cf4-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cf4-119">Read-only.</span></span>|
|<span data-ttu-id="16cf4-120">id</span><span class="sxs-lookup"><span data-stu-id="16cf4-120">id</span></span>|<span data-ttu-id="16cf4-121">String</span><span class="sxs-lookup"><span data-stu-id="16cf4-121">String</span></span>|<span data-ttu-id="16cf4-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cf4-122">Read-only.</span></span>|
|<span data-ttu-id="16cf4-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="16cf4-123">isDefault</span></span>|<span data-ttu-id="16cf4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="16cf4-124">Boolean</span></span>|<span data-ttu-id="16cf4-125">Указывает, является ли это файл соглашения по умолчанию, если ни одна из культур не соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="16cf4-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="16cf4-126">Если ни один из файлов не помечен как файл по умолчанию, первый из них будет рассматриваться как файл по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="16cf4-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="16cf4-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cf4-127">Read-only.</span></span>|
|<span data-ttu-id="16cf4-128">language</span><span class="sxs-lookup"><span data-stu-id="16cf4-128">language</span></span>|<span data-ttu-id="16cf4-129">String</span><span class="sxs-lookup"><span data-stu-id="16cf4-129">String</span></span>|<span data-ttu-id="16cf4-130">Язык и формат файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="16cf4-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="16cf4-131">languagecode2 — это двух буквный код нижнего регистра, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="16cf4-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="16cf4-132">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="16cf4-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="16cf4-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cf4-133">Read-only.</span></span>|
|<span data-ttu-id="16cf4-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="16cf4-134">isMajorVersion</span></span>|<span data-ttu-id="16cf4-135">Логический</span><span class="sxs-lookup"><span data-stu-id="16cf4-135">Boolean</span></span>|<span data-ttu-id="16cf4-136">Указывает, является ли файл соглашения основным обновлением версии.</span><span class="sxs-lookup"><span data-stu-id="16cf4-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="16cf4-137">Обновления основных версий аннулируют принятие соглашения на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="16cf4-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="16cf4-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16cf4-138">createdDateTime</span></span>|<span data-ttu-id="16cf4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16cf4-139">DateTimeOffset</span></span>|<span data-ttu-id="16cf4-140">Дата создания файла.</span><span class="sxs-lookup"><span data-stu-id="16cf4-140">The date time representing when the file was created.</span></span> <span data-ttu-id="16cf4-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="16cf4-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="16cf4-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="16cf4-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="16cf4-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16cf4-143">JSON representation</span></span>

<span data-ttu-id="16cf4-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16cf4-144">The following is a JSON representation of the resource.</span></span>

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


