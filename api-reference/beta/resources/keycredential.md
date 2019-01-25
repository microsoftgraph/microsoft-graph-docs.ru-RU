---
title: Тип ресурса keyCredential
description: Содержит основные учетных данных, связанных с приложением или участников-служб. Свойство **keyCredentials** сущности, приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519054"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c6f26-104">Тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="c6f26-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f26-105">Содержит основные учетных данных, связанных с приложением или участников-служб.</span><span class="sxs-lookup"><span data-stu-id="c6f26-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="c6f26-106">Свойство **keyCredentials** сущности, [приложения](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="c6f26-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c6f26-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6f26-107">JSON representation</span></span>

<span data-ttu-id="c6f26-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c6f26-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="c6f26-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6f26-109">Properties</span></span>
| <span data-ttu-id="c6f26-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6f26-110">Property</span></span>     | <span data-ttu-id="c6f26-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c6f26-111">Type</span></span>   |<span data-ttu-id="c6f26-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c6f26-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6f26-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c6f26-113">customKeyIdentifier</span></span>|<span data-ttu-id="c6f26-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c6f26-114">Binary</span></span>| <span data-ttu-id="c6f26-115">Настраиваемые идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="c6f26-115">Custom key identifier</span></span> |
|<span data-ttu-id="c6f26-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f26-116">endDateTime</span></span>|<span data-ttu-id="c6f26-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6f26-117">DateTimeOffset</span></span>|<span data-ttu-id="c6f26-118">Дата и время истечения срока действия учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c6f26-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c6f26-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c6f26-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c6f26-120">Идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="c6f26-120">keyId</span></span>|<span data-ttu-id="c6f26-121">Guid</span><span class="sxs-lookup"><span data-stu-id="c6f26-121">Guid</span></span>|<span data-ttu-id="c6f26-122">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="c6f26-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c6f26-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f26-123">startDateTime</span></span>|<span data-ttu-id="c6f26-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6f26-124">DateTimeOffset</span></span>|<span data-ttu-id="c6f26-125">Дата и время, в которой действителен учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c6f26-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c6f26-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c6f26-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c6f26-127">type</span><span class="sxs-lookup"><span data-stu-id="c6f26-127">type</span></span>|<span data-ttu-id="c6f26-128">String</span><span class="sxs-lookup"><span data-stu-id="c6f26-128">String</span></span>|<span data-ttu-id="c6f26-129">Тип ключа учетных данных; Например, «Симметричные».</span><span class="sxs-lookup"><span data-stu-id="c6f26-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c6f26-130">USAGE</span><span class="sxs-lookup"><span data-stu-id="c6f26-130">usage</span></span>|<span data-ttu-id="c6f26-131">String</span><span class="sxs-lookup"><span data-stu-id="c6f26-131">String</span></span>|<span data-ttu-id="c6f26-132">Строка, описывающая назначение, для которого можно использовать ключ; например «проверка».</span><span class="sxs-lookup"><span data-stu-id="c6f26-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c6f26-133">key</span><span class="sxs-lookup"><span data-stu-id="c6f26-133">key</span></span>|<span data-ttu-id="c6f26-134">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c6f26-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keycredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
