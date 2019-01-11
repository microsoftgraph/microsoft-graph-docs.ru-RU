---
title: Тип ресурса agreementFile
description: Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD). Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).
localization_priority: Normal
ms.openlocfilehash: f06792d63deabf25659a09e8aec5ed0e8f036472
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804510"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="a161f-104">Тип ресурса agreementFile</span><span class="sxs-lookup"><span data-stu-id="a161f-104">agreementFile resource type</span></span>

> <span data-ttu-id="a161f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a161f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a161f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a161f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a161f-107">Представляет настраиваемое условия использования соглашения файл, который управляет клиента с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a161f-107">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a161f-108">Содержит метаданные о файле соглашения (например, имя, язык, и его файл по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="a161f-108">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="a161f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a161f-109">Properties</span></span>
| <span data-ttu-id="a161f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a161f-110">Property</span></span>     | <span data-ttu-id="a161f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a161f-111">Type</span></span>        | <span data-ttu-id="a161f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a161f-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a161f-113">fileData</span><span class="sxs-lookup"><span data-stu-id="a161f-113">fileData</span></span>|[<span data-ttu-id="a161f-114">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="a161f-114">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="a161f-115">Данные, представляющие условия использования PDF-документа.</span><span class="sxs-lookup"><span data-stu-id="a161f-115">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="a161f-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a161f-116">Read-only.</span></span>|
|<span data-ttu-id="a161f-117">fileName</span><span class="sxs-lookup"><span data-stu-id="a161f-117">fileName</span></span>|<span data-ttu-id="a161f-118">String</span><span class="sxs-lookup"><span data-stu-id="a161f-118">String</span></span>|<span data-ttu-id="a161f-119">Имя файла соглашения (например, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="a161f-119">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="a161f-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a161f-120">Read-only.</span></span>|
|<span data-ttu-id="a161f-121">id</span><span class="sxs-lookup"><span data-stu-id="a161f-121">id</span></span>|<span data-ttu-id="a161f-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a161f-122">String</span></span>|<span data-ttu-id="a161f-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a161f-123">Read-only.</span></span>|
|<span data-ttu-id="a161f-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="a161f-124">isDefault</span></span>|<span data-ttu-id="a161f-125">Логический</span><span class="sxs-lookup"><span data-stu-id="a161f-125">Boolean</span></span>|<span data-ttu-id="a161f-126">Указывает, является ли файл соглашения по умолчанию Если ни одна из культур совпадает с клиентом.</span><span class="sxs-lookup"><span data-stu-id="a161f-126">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="a161f-127">Если ни один из файлов помечены как по умолчанию, первый будет рассматриваться как значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a161f-127">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="a161f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a161f-128">Read-only.</span></span>|
|<span data-ttu-id="a161f-129">language</span><span class="sxs-lookup"><span data-stu-id="a161f-129">language</span></span>|<span data-ttu-id="a161f-130">String</span><span class="sxs-lookup"><span data-stu-id="a161f-130">String</span></span>|<span data-ttu-id="a161f-131">Язык и региональные параметры соглашения файла в формате languagecode2-страны/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="a161f-131">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="a161f-132">languagecode2 — это строчная двухбуквенный код, производный от ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="a161f-132">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="a161f-133">Страна/regioncode2 является производным от ISO 3166 и обычно состоит из двух прописных букв или тег языка BCP 47 (например, en US).</span><span class="sxs-lookup"><span data-stu-id="a161f-133">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="a161f-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a161f-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a161f-135">Связи</span><span class="sxs-lookup"><span data-stu-id="a161f-135">Relationships</span></span>
<span data-ttu-id="a161f-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a161f-136">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a161f-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a161f-137">JSON representation</span></span>

<span data-ttu-id="a161f-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a161f-138">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
