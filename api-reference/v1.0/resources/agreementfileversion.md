---
title: тип ресурса agreementFileVersion
description: Представляет настраиваемую версию локализованных файлов политик условий соглашения об использовании в Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: rajadineshmurugesan-microsoft
ms.openlocfilehash: 84358a8795022ab948e3f554d5f3d08a9e173cd7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722724"
---
# <a name="agreementfileversion-resource-type"></a><span data-ttu-id="5b85a-103">тип ресурса agreementFileVersion</span><span class="sxs-lookup"><span data-stu-id="5b85a-103">agreementFileVersion resource type</span></span>

<span data-ttu-id="5b85a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b85a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b85a-105">Представляет настраиваемую версию файла соглашений об использовании, который клиент управляет с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="5b85a-105">Represents a customized version of terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="5b85a-106">Он содержит метаданные о файле соглашения (например, имя, язык и является ли это файл по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="5b85a-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="5b85a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b85a-107">Properties</span></span>
| <span data-ttu-id="5b85a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b85a-108">Property</span></span>     | <span data-ttu-id="5b85a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b85a-109">Type</span></span>        | <span data-ttu-id="5b85a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b85a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b85a-111">fileData</span><span class="sxs-lookup"><span data-stu-id="5b85a-111">fileData</span></span>|[<span data-ttu-id="5b85a-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="5b85a-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="5b85a-113">Данные, которые представляют условия использования документа PDF.</span><span class="sxs-lookup"><span data-stu-id="5b85a-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="5b85a-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b85a-114">Read-only.</span></span>|
|<span data-ttu-id="5b85a-115">fileName</span><span class="sxs-lookup"><span data-stu-id="5b85a-115">fileName</span></span>|<span data-ttu-id="5b85a-116">String</span><span class="sxs-lookup"><span data-stu-id="5b85a-116">String</span></span>|<span data-ttu-id="5b85a-117">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="5b85a-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="5b85a-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b85a-118">Read-only.</span></span>|
|<span data-ttu-id="5b85a-119">id</span><span class="sxs-lookup"><span data-stu-id="5b85a-119">id</span></span>|<span data-ttu-id="5b85a-120">String</span><span class="sxs-lookup"><span data-stu-id="5b85a-120">String</span></span>|<span data-ttu-id="5b85a-121">Идентификатор объекта AgreementFileVersion.</span><span class="sxs-lookup"><span data-stu-id="5b85a-121">The identifier of the agreementFileVersion object.</span></span> <span data-ttu-id="5b85a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b85a-122">Read-only.</span></span>|
|<span data-ttu-id="5b85a-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="5b85a-123">isDefault</span></span>|<span data-ttu-id="5b85a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b85a-124">Boolean</span></span>|<span data-ttu-id="5b85a-125">Если ни один из языков не соответствует предпочтениям клиента, указывает, является ли это файл соглашения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5b85a-125">If none of the languages matches the client preference, indicates whether this is the default agreement file .</span></span> <span data-ttu-id="5b85a-126">Если ни один из файлов не помечен как по умолчанию, первый из них рассматривается как по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5b85a-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="5b85a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b85a-127">Read-only.</span></span>|
|<span data-ttu-id="5b85a-128">language</span><span class="sxs-lookup"><span data-stu-id="5b85a-128">language</span></span>|<span data-ttu-id="5b85a-129">String</span><span class="sxs-lookup"><span data-stu-id="5b85a-129">String</span></span>|<span data-ttu-id="5b85a-130">Язык файла соглашения в формате languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="5b85a-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="5b85a-131">languagecode2 — это код из двух букв более низкого уровня, полученный из ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="5b85a-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="5b85a-132">country/regioncode2 является производным от ISO 3166 и обычно состоит из двух верхних букв или языкового тега BCP-47 (например, en-US).</span><span class="sxs-lookup"><span data-stu-id="5b85a-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="5b85a-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b85a-133">Read-only.</span></span>|
|<span data-ttu-id="5b85a-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="5b85a-134">isMajorVersion</span></span>|<span data-ttu-id="5b85a-135">Логический</span><span class="sxs-lookup"><span data-stu-id="5b85a-135">Boolean</span></span>|<span data-ttu-id="5b85a-136">Указывает, является ли файл соглашения основным обновлением версии.</span><span class="sxs-lookup"><span data-stu-id="5b85a-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="5b85a-137">Обновления основных версий недействительны для принятия соглашения на соответствующем языке.</span><span class="sxs-lookup"><span data-stu-id="5b85a-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="5b85a-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b85a-138">createdDateTime</span></span>|<span data-ttu-id="5b85a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b85a-139">DateTimeOffset</span></span>|<span data-ttu-id="5b85a-140">Время даты, представляющее момент создания файла. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="5b85a-140">The date time representing when the file was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b85a-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="5b85a-141">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b85a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b85a-142">JSON representation</span></span>

<span data-ttu-id="5b85a-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b85a-143">The following is a JSON representation of the resource.</span></span>

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
