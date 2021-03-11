---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cc6d66a4361f760b702844991e6fdc3f590c4007
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721490"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="94c16-104">тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="94c16-104">keyCredential resource type</span></span>

<span data-ttu-id="94c16-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94c16-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c16-106">Содержит ключевые учетные данные, связанные с приложением или директором службы.</span><span class="sxs-lookup"><span data-stu-id="94c16-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="94c16-107">Свойство **keyCredentials** сущностями приложения и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**. [](application.md)</span><span class="sxs-lookup"><span data-stu-id="94c16-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="94c16-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="94c16-108">Properties</span></span>
| <span data-ttu-id="94c16-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="94c16-109">Property</span></span>     | <span data-ttu-id="94c16-110">Тип</span><span class="sxs-lookup"><span data-stu-id="94c16-110">Type</span></span>   |<span data-ttu-id="94c16-111">Описание</span><span class="sxs-lookup"><span data-stu-id="94c16-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94c16-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="94c16-112">customKeyIdentifier</span></span>|<span data-ttu-id="94c16-113">Binary</span><span class="sxs-lookup"><span data-stu-id="94c16-113">Binary</span></span>| <span data-ttu-id="94c16-114">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="94c16-114">Custom key identifier</span></span> |
| <span data-ttu-id="94c16-115">displayName</span><span class="sxs-lookup"><span data-stu-id="94c16-115">displayName</span></span> | <span data-ttu-id="94c16-116">String</span><span class="sxs-lookup"><span data-stu-id="94c16-116">String</span></span> | <span data-ttu-id="94c16-117">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="94c16-117">Friendly name for the key.</span></span> <span data-ttu-id="94c16-118">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="94c16-118">Optional.</span></span> |
|<span data-ttu-id="94c16-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="94c16-119">endDateTime</span></span>|<span data-ttu-id="94c16-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c16-120">DateTimeOffset</span></span>|<span data-ttu-id="94c16-121">Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="94c16-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94c16-122">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="94c16-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="94c16-123">keyId</span><span class="sxs-lookup"><span data-stu-id="94c16-123">keyId</span></span>|<span data-ttu-id="94c16-124">Guid</span><span class="sxs-lookup"><span data-stu-id="94c16-124">Guid</span></span>|<span data-ttu-id="94c16-125">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="94c16-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="94c16-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="94c16-126">startDateTime</span></span>|<span data-ttu-id="94c16-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94c16-127">DateTimeOffset</span></span>|<span data-ttu-id="94c16-128">Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="94c16-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94c16-129">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="94c16-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="94c16-130">type</span><span class="sxs-lookup"><span data-stu-id="94c16-130">type</span></span>|<span data-ttu-id="94c16-131">String</span><span class="sxs-lookup"><span data-stu-id="94c16-131">String</span></span>|<span data-ttu-id="94c16-132">Тип учетных данных ключей; например, "Симметричный".</span><span class="sxs-lookup"><span data-stu-id="94c16-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="94c16-133">использование</span><span class="sxs-lookup"><span data-stu-id="94c16-133">usage</span></span>|<span data-ttu-id="94c16-134">String</span><span class="sxs-lookup"><span data-stu-id="94c16-134">String</span></span>|<span data-ttu-id="94c16-135">Строка, описываемая цель, для которой можно использовать ключ; например, "Проверка".</span><span class="sxs-lookup"><span data-stu-id="94c16-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="94c16-136">key</span><span class="sxs-lookup"><span data-stu-id="94c16-136">key</span></span>|<span data-ttu-id="94c16-137">Двоичный</span><span class="sxs-lookup"><span data-stu-id="94c16-137">Binary</span></span>| <span data-ttu-id="94c16-138">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="94c16-138">Value for the key credential.</span></span> <span data-ttu-id="94c16-139">Должно быть базовым значением 64.</span><span class="sxs-lookup"><span data-stu-id="94c16-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94c16-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94c16-140">JSON representation</span></span>

<span data-ttu-id="94c16-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94c16-141">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


