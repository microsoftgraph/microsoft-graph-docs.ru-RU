---
title: Тип ресурса Агриментфиле
description: Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD). Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea78059ecf29f1cadb9634492ced726775f5614d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508375"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="0ca29-104">Тип ресурса Агриментфиле</span><span class="sxs-lookup"><span data-stu-id="0ca29-104">agreementFile resource type</span></span>

<span data-ttu-id="0ca29-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ca29-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca29-106">Представляет настраиваемый термин файла соглашения об использовании, который клиент управляет с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0ca29-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="0ca29-107">Он содержит метаданные о файле соглашения (например, имя, язык и является ли он файлом по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="0ca29-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="0ca29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ca29-108">Properties</span></span>
| <span data-ttu-id="0ca29-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ca29-109">Property</span></span>     | <span data-ttu-id="0ca29-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0ca29-110">Type</span></span>        | <span data-ttu-id="0ca29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ca29-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ca29-112">fileData</span><span class="sxs-lookup"><span data-stu-id="0ca29-112">fileData</span></span>|[<span data-ttu-id="0ca29-113">агриментфиледата</span><span class="sxs-lookup"><span data-stu-id="0ca29-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="0ca29-114">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="0ca29-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="0ca29-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ca29-115">Read-only.</span></span>|
|<span data-ttu-id="0ca29-116">fileName</span><span class="sxs-lookup"><span data-stu-id="0ca29-116">fileName</span></span>|<span data-ttu-id="0ca29-117">String</span><span class="sxs-lookup"><span data-stu-id="0ca29-117">String</span></span>|<span data-ttu-id="0ca29-118">Имя файла соглашения (например, Тау. PDF).</span><span class="sxs-lookup"><span data-stu-id="0ca29-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="0ca29-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ca29-119">Read-only.</span></span>|
|<span data-ttu-id="0ca29-120">id</span><span class="sxs-lookup"><span data-stu-id="0ca29-120">id</span></span>|<span data-ttu-id="0ca29-121">String</span><span class="sxs-lookup"><span data-stu-id="0ca29-121">String</span></span>|<span data-ttu-id="0ca29-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ca29-122">Read-only.</span></span>|
|<span data-ttu-id="0ca29-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="0ca29-123">isDefault</span></span>|<span data-ttu-id="0ca29-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ca29-124">Boolean</span></span>|<span data-ttu-id="0ca29-125">Указывает, является ли этот файл соглашением по умолчанию, если ни одна из культур не соответствует параметрам клиента.</span><span class="sxs-lookup"><span data-stu-id="0ca29-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="0ca29-126">Если ни один из файлов не помечен как используемый по умолчанию, первый из них будет считаться используемым по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0ca29-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="0ca29-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ca29-127">Read-only.</span></span>|
|<span data-ttu-id="0ca29-128">language</span><span class="sxs-lookup"><span data-stu-id="0ca29-128">language</span></span>|<span data-ttu-id="0ca29-129">String</span><span class="sxs-lookup"><span data-stu-id="0ca29-129">String</span></span>|<span data-ttu-id="0ca29-130">Язык и региональные параметры файла соглашения в формате languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="0ca29-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="0ca29-131">languagecode2 это код из двух букв в нижнем регистре, производный от стандарта ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="0ca29-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="0ca29-132">страна или regioncode2 является производной от стандарта ISO 3166 и обычно состоит из двух прописных букв или тега языка BCP-47 (например, EN-US).</span><span class="sxs-lookup"><span data-stu-id="0ca29-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="0ca29-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ca29-133">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ca29-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ca29-134">Relationships</span></span>
<span data-ttu-id="0ca29-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ca29-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0ca29-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ca29-136">JSON representation</span></span>

<span data-ttu-id="0ca29-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ca29-137">The following is a JSON representation of the resource.</span></span>

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
