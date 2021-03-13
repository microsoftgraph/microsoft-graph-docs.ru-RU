---
title: тип ресурса agreementFileVersion
description: Представляет настраиваемую версию локализованных файлов политик условий соглашения об использовании в Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: afdfe9ce0e5440218919d0b019da6cbfe21a472f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761893"
---
# <a name="agreementfileversion-resource-type"></a><span data-ttu-id="8f7f3-104">тип ресурса agreementFileVersion</span><span class="sxs-lookup"><span data-stu-id="8f7f3-104">agreementFileVersion resource type</span></span>

<span data-ttu-id="8f7f3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f7f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f7f3-106">Представляет настраиваемую версию файла соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8f7f3-106">Represents a customized version of terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="8f7f3-107">Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="8f7f3-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f7f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f7f3-108">Properties</span></span>
| <span data-ttu-id="8f7f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f7f3-109">Property</span></span>     | <span data-ttu-id="8f7f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8f7f3-110">Type</span></span>        | <span data-ttu-id="8f7f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f7f3-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f7f3-112">fileData</span><span class="sxs-lookup"><span data-stu-id="8f7f3-112">fileData</span></span>|[<span data-ttu-id="8f7f3-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="8f7f3-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="8f7f3-114">Данные, представляющие условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="8f7f3-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-115">Read-only.</span></span>|
|<span data-ttu-id="8f7f3-116">fileName</span><span class="sxs-lookup"><span data-stu-id="8f7f3-116">fileName</span></span>|<span data-ttu-id="8f7f3-117">String</span><span class="sxs-lookup"><span data-stu-id="8f7f3-117">String</span></span>|<span data-ttu-id="8f7f3-118">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="8f7f3-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="8f7f3-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-119">Read-only.</span></span>|
|<span data-ttu-id="8f7f3-120">id</span><span class="sxs-lookup"><span data-stu-id="8f7f3-120">id</span></span>|<span data-ttu-id="8f7f3-121">String</span><span class="sxs-lookup"><span data-stu-id="8f7f3-121">String</span></span>|<span data-ttu-id="8f7f3-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-122">Read-only.</span></span>|
|<span data-ttu-id="8f7f3-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="8f7f3-123">isDefault</span></span>|<span data-ttu-id="8f7f3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f7f3-124">Boolean</span></span>|<span data-ttu-id="8f7f3-125">Указывает, является ли это файл соглашения по умолчанию, если ни одна из культур не соответствует предпочтениям клиента.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="8f7f3-126">Если ни один из файлов не помечен как по умолчанию, первый будет рассматриваться как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="8f7f3-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-127">Read-only.</span></span>|
|<span data-ttu-id="8f7f3-128">language</span><span class="sxs-lookup"><span data-stu-id="8f7f3-128">language</span></span>|<span data-ttu-id="8f7f3-129">String</span><span class="sxs-lookup"><span data-stu-id="8f7f3-129">String</span></span>|<span data-ttu-id="8f7f3-130">Культура файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="8f7f3-131">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="8f7f3-132">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="8f7f3-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="8f7f3-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-133">Read-only.</span></span>|
|<span data-ttu-id="8f7f3-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="8f7f3-134">isMajorVersion</span></span>|<span data-ttu-id="8f7f3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f7f3-135">Boolean</span></span>|<span data-ttu-id="8f7f3-136">Указывает, является ли файл соглашения основным обновлением версии.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="8f7f3-137">Обновления основных версий недействительны для принятия соглашения на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="8f7f3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f7f3-138">createdDateTime</span></span>|<span data-ttu-id="8f7f3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f7f3-139">DateTimeOffset</span></span>|<span data-ttu-id="8f7f3-140">Время даты, представляющее момент создания файла. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-140">The date time representing when the file was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f7f3-141">Например, полночь UTC 1 января 2014 г. это: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-141">For example, midnight UTC on Jan 1, 2014 is: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="8f7f3-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8f7f3-142">displayName</span></span>|<span data-ttu-id="8f7f3-143">String</span><span class="sxs-lookup"><span data-stu-id="8f7f3-143">String</span></span>|<span data-ttu-id="8f7f3-144">Локализованное отображение имени файла политики соглашения.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-144">Localized display name of the policy file of an agreement.</span></span> <span data-ttu-id="8f7f3-145">Локализованное имя отображения отображается конечным пользователям, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-145">The localized display name is shown to end users who view the agreement.</span></span>

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a><span data-ttu-id="8f7f3-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f7f3-146">JSON representation</span></span>

<span data-ttu-id="8f7f3-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f7f3-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileVersion"
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
