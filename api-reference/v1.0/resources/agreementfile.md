---
title: тип ресурса agreementFile
description: Представляет настраиваемый файл соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 843870db12d9cdec518c18288adce76ea4b2dcf5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761746"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="cf1e5-103">тип ресурса agreementFile</span><span class="sxs-lookup"><span data-stu-id="cf1e5-103">agreementFile resource type</span></span>

<span data-ttu-id="cf1e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf1e5-105">Представляет настраиваемый файл соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cf1e5-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="cf1e5-106">Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="cf1e5-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="cf1e5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf1e5-107">Properties</span></span>
| <span data-ttu-id="cf1e5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf1e5-108">Property</span></span>     | <span data-ttu-id="cf1e5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cf1e5-109">Type</span></span>        | <span data-ttu-id="cf1e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cf1e5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf1e5-111">fileData</span><span class="sxs-lookup"><span data-stu-id="cf1e5-111">fileData</span></span>|[<span data-ttu-id="cf1e5-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="cf1e5-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="cf1e5-113">Данные, которые представляют условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="cf1e5-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-114">Read-only.</span></span>|
|<span data-ttu-id="cf1e5-115">fileName</span><span class="sxs-lookup"><span data-stu-id="cf1e5-115">fileName</span></span>|<span data-ttu-id="cf1e5-116">String</span><span class="sxs-lookup"><span data-stu-id="cf1e5-116">String</span></span>|<span data-ttu-id="cf1e5-117">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="cf1e5-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="cf1e5-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-118">Read-only.</span></span>|
|<span data-ttu-id="cf1e5-119">id</span><span class="sxs-lookup"><span data-stu-id="cf1e5-119">id</span></span>|<span data-ttu-id="cf1e5-120">String</span><span class="sxs-lookup"><span data-stu-id="cf1e5-120">String</span></span>|<span data-ttu-id="cf1e5-121">Идентификатор файла соглашения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-121">The identifier of the agreement file.</span></span> <span data-ttu-id="cf1e5-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-122">Read-only.</span></span>|
|<span data-ttu-id="cf1e5-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="cf1e5-123">isDefault</span></span>|<span data-ttu-id="cf1e5-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf1e5-124">Boolean</span></span>|<span data-ttu-id="cf1e5-125">Если ни один из языков не соответствует предпочтениям клиента, указывает, что это файл соглашения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-125">If none of the languages matches the client preference, indicates that this is the default agreement file.</span></span> <span data-ttu-id="cf1e5-126">Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="cf1e5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-127">Read-only.</span></span>|
|<span data-ttu-id="cf1e5-128">language</span><span class="sxs-lookup"><span data-stu-id="cf1e5-128">language</span></span>|<span data-ttu-id="cf1e5-129">String</span><span class="sxs-lookup"><span data-stu-id="cf1e5-129">String</span></span>|<span data-ttu-id="cf1e5-130">Язык файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="cf1e5-131">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="cf1e5-132">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="cf1e5-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="cf1e5-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-133">Read-only.</span></span>|
|<span data-ttu-id="cf1e5-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="cf1e5-134">isMajorVersion</span></span>|<span data-ttu-id="cf1e5-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf1e5-135">Boolean</span></span>|<span data-ttu-id="cf1e5-136">Указывает, является ли файл соглашения основным обновлением версии.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="cf1e5-137">Обновления основных версий недействительны для принятия соглашения на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="cf1e5-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf1e5-138">createdDateTime</span></span>|<span data-ttu-id="cf1e5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1e5-139">DateTimeOffset</span></span>|<span data-ttu-id="cf1e5-140">Время даты, представляющее момент создания файла.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-140">The date time representing when the file was created.</span></span> <span data-ttu-id="cf1e5-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cf1e5-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cf1e5-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="cf1e5-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="cf1e5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cf1e5-143">displayName</span></span>|<span data-ttu-id="cf1e5-144">String</span><span class="sxs-lookup"><span data-stu-id="cf1e5-144">String</span></span>|<span data-ttu-id="cf1e5-145">Локализованное отображение имени файла политики соглашения.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-145">Localized display name of the policy file of an agreement.</span></span> <span data-ttu-id="cf1e5-146">Локализованное имя отображения отображается конечным пользователям, которые просматривают соглашение.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-146">The localized display name is shown to end users who view the agreement.</span></span>

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="cf1e5-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf1e5-147">JSON representation</span></span>

<span data-ttu-id="cf1e5-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf1e5-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


