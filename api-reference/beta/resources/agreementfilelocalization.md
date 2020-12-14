---
title: Тип ресурса agreementFileLocalization
description: Представляет локализованные файлы политик соглашения об условиях использования в Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык и то, является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 7daadaa82fe7a15c534e1fc359791d61bf1db669
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664120"
---
# <a name="agreementfilelocalization-resource-type"></a><span data-ttu-id="3d352-104">Тип ресурса agreementFileLocalization</span><span class="sxs-lookup"><span data-stu-id="3d352-104">agreementFileLocalization resource type</span></span>

<span data-ttu-id="3d352-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d352-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d352-106">Представляет настраиваемый файл соглашений об условиях использования, управляемый клиентом с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3d352-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="3d352-107">Содержит метаданные о файле соглашения (например, имя, язык и то, является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="3d352-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create agreementFileLocalization](../api/agreementfilelocalization-post-agreementfilelocalizations.md) | [agreementfilelocalization](agreementfilelocalization.md) | Create a new agreementFileLocalization. |
| [List agreementFileLocalizations](../api/agreementfilelocalization-list.md) | [agreementfilelocalization](agreementfilelocalization.md) collection | Get an agreementFileLocalization object collection. |
| [Get agreementFileLocalization](../api/agreementfilelocalization-get.md) | [agreementfilelocalization](agreementfilelocalization.md) | Read properties and relationships of an agreementFileLocalization object. |
| [List agreementFileVersions](../api/agreementfileversion-list.md) | [agreementfileversion](agreementfileversion.md) collection | Get an agreementFileVersion object collection. |
| [Get agreementFileVersion](../api/agreementfileversion-get.md) | [agreementfileversion](agreementfileversion.md) | Read properties and relationships of an agreementFileVersion object. |
-->

## <a name="properties"></a><span data-ttu-id="3d352-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d352-108">Properties</span></span>
| <span data-ttu-id="3d352-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d352-109">Property</span></span>     | <span data-ttu-id="3d352-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d352-110">Type</span></span>        | <span data-ttu-id="3d352-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d352-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d352-112">fileData</span><span class="sxs-lookup"><span data-stu-id="3d352-112">fileData</span></span>|[<span data-ttu-id="3d352-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="3d352-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="3d352-114">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="3d352-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="3d352-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d352-115">Read-only.</span></span>|
|<span data-ttu-id="3d352-116">fileName</span><span class="sxs-lookup"><span data-stu-id="3d352-116">fileName</span></span>|<span data-ttu-id="3d352-117">String</span><span class="sxs-lookup"><span data-stu-id="3d352-117">String</span></span>|<span data-ttu-id="3d352-118">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="3d352-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="3d352-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d352-119">Read-only.</span></span>|
|<span data-ttu-id="3d352-120">id</span><span class="sxs-lookup"><span data-stu-id="3d352-120">id</span></span>|<span data-ttu-id="3d352-121">String</span><span class="sxs-lookup"><span data-stu-id="3d352-121">String</span></span>|<span data-ttu-id="3d352-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d352-122">Read-only.</span></span>|
|<span data-ttu-id="3d352-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="3d352-123">isDefault</span></span>|<span data-ttu-id="3d352-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d352-124">Boolean</span></span>|<span data-ttu-id="3d352-125">Указывает, является ли это файл соглашения по умолчанию, если ни одна из культур не соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="3d352-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="3d352-126">Если ни один из файлов не помечен как файл по умолчанию, первый из них будет рассматриваться как файл по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3d352-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="3d352-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d352-127">Read-only.</span></span>|
|<span data-ttu-id="3d352-128">language</span><span class="sxs-lookup"><span data-stu-id="3d352-128">language</span></span>|<span data-ttu-id="3d352-129">String</span><span class="sxs-lookup"><span data-stu-id="3d352-129">String</span></span>|<span data-ttu-id="3d352-130">Язык и формат файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="3d352-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="3d352-131">languagecode2 — это двух буквный код нижнего регистра, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="3d352-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="3d352-132">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="3d352-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="3d352-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d352-133">Read-only.</span></span>|
|<span data-ttu-id="3d352-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="3d352-134">isMajorVersion</span></span>|<span data-ttu-id="3d352-135">Логический</span><span class="sxs-lookup"><span data-stu-id="3d352-135">Boolean</span></span>|<span data-ttu-id="3d352-136">Указывает, является ли файл соглашения обновлением основной версии.</span><span class="sxs-lookup"><span data-stu-id="3d352-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="3d352-137">Обновления основных версий аннулируют принятие соглашения на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="3d352-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="3d352-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d352-138">createdDateTime</span></span>|<span data-ttu-id="3d352-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d352-139">DateTimeOffset</span></span>|<span data-ttu-id="3d352-140">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="3d352-140">The date time representing when the file was created.</span></span> <span data-ttu-id="3d352-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3d352-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3d352-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="3d352-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a><span data-ttu-id="3d352-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d352-143">JSON representation</span></span>

<span data-ttu-id="3d352-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d352-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
