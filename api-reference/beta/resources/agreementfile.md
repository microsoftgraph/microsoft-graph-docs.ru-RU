---
title: Тип ресурса Агриментфиле
description: Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
ms.openlocfilehash: b914feecfc91d71c525711f725bf4a533d44a6b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328624"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="567c1-104">Тип ресурса Агриментфиле</span><span class="sxs-lookup"><span data-stu-id="567c1-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="567c1-105">Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="567c1-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="567c1-106">Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="567c1-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="567c1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="567c1-107">Properties</span></span>
| <span data-ttu-id="567c1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="567c1-108">Property</span></span>     | <span data-ttu-id="567c1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="567c1-109">Type</span></span>        | <span data-ttu-id="567c1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="567c1-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="567c1-111">fileData</span><span class="sxs-lookup"><span data-stu-id="567c1-111">fileData</span></span>|[<span data-ttu-id="567c1-112">Агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="567c1-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="567c1-113">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="567c1-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="567c1-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="567c1-114">Read-only.</span></span>|
|<span data-ttu-id="567c1-115">fileName</span><span class="sxs-lookup"><span data-stu-id="567c1-115">fileName</span></span>|<span data-ttu-id="567c1-116">String</span><span class="sxs-lookup"><span data-stu-id="567c1-116">String</span></span>|<span data-ttu-id="567c1-117">Имя файла соглашения (например, Тау. PDF).</span><span class="sxs-lookup"><span data-stu-id="567c1-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="567c1-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="567c1-118">Read-only.</span></span>|
|<span data-ttu-id="567c1-119">id</span><span class="sxs-lookup"><span data-stu-id="567c1-119">id</span></span>|<span data-ttu-id="567c1-120">String</span><span class="sxs-lookup"><span data-stu-id="567c1-120">String</span></span>|<span data-ttu-id="567c1-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="567c1-121">Read-only.</span></span>|
|<span data-ttu-id="567c1-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="567c1-122">isDefault</span></span>|<span data-ttu-id="567c1-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="567c1-123">Boolean</span></span>|<span data-ttu-id="567c1-124">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="567c1-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="567c1-125">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="567c1-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="567c1-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="567c1-126">Read-only.</span></span>|
|<span data-ttu-id="567c1-127">language</span><span class="sxs-lookup"><span data-stu-id="567c1-127">language</span></span>|<span data-ttu-id="567c1-128">String</span><span class="sxs-lookup"><span data-stu-id="567c1-128">String</span></span>|<span data-ttu-id="567c1-129">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="567c1-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="567c1-130">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="567c1-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="567c1-131">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="567c1-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="567c1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="567c1-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="567c1-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="567c1-133">Relationships</span></span>
<span data-ttu-id="567c1-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="567c1-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="567c1-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="567c1-135">JSON representation</span></span>

<span data-ttu-id="567c1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="567c1-136">The following is a JSON representation of the resource.</span></span>

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
