---
title: Тип ресурса keyCredential
description: Содержит учетные данные ключа, связанные с приложением или основным компонентом-службой. Свойство **keyCredentials** объектов application и servicePrincipal — это коллекция **объектов keyCredential.**
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 7ba1bfbf5a3769163a2e9c839b568f22f33f9ac8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135438"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c5f31-104">Тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="c5f31-104">keyCredential resource type</span></span>

<span data-ttu-id="c5f31-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f31-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f31-106">Содержит учетные данные ключа, связанные с приложением или основным компонентом-службой.</span><span class="sxs-lookup"><span data-stu-id="c5f31-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="c5f31-107">Свойство **keyCredentials** объектов [application](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **объектов keyCredential.**</span><span class="sxs-lookup"><span data-stu-id="c5f31-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="c5f31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5f31-108">Properties</span></span>
| <span data-ttu-id="c5f31-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5f31-109">Property</span></span>     | <span data-ttu-id="c5f31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c5f31-110">Type</span></span>   |<span data-ttu-id="c5f31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5f31-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5f31-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5f31-112">customKeyIdentifier</span></span>|<span data-ttu-id="c5f31-113">Binary</span><span class="sxs-lookup"><span data-stu-id="c5f31-113">Binary</span></span>| <span data-ttu-id="c5f31-114">Идентификатор пользовательского ключа</span><span class="sxs-lookup"><span data-stu-id="c5f31-114">Custom key identifier</span></span> |
| <span data-ttu-id="c5f31-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c5f31-115">displayName</span></span> | <span data-ttu-id="c5f31-116">Строка</span><span class="sxs-lookup"><span data-stu-id="c5f31-116">String</span></span> | <span data-ttu-id="c5f31-117">Имя ключа.</span><span class="sxs-lookup"><span data-stu-id="c5f31-117">Friendly name for the key.</span></span> <span data-ttu-id="c5f31-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c5f31-118">Optional.</span></span> |
|<span data-ttu-id="c5f31-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f31-119">endDateTime</span></span>|<span data-ttu-id="c5f31-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f31-120">DateTimeOffset</span></span>|<span data-ttu-id="c5f31-121">Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c5f31-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5f31-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5f31-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c5f31-123">keyId</span><span class="sxs-lookup"><span data-stu-id="c5f31-123">keyId</span></span>|<span data-ttu-id="c5f31-124">Guid</span><span class="sxs-lookup"><span data-stu-id="c5f31-124">Guid</span></span>|<span data-ttu-id="c5f31-125">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="c5f31-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c5f31-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f31-126">startDateTime</span></span>|<span data-ttu-id="c5f31-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f31-127">DateTimeOffset</span></span>|<span data-ttu-id="c5f31-128">Дата и время, когда учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c5f31-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5f31-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5f31-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c5f31-130">type</span><span class="sxs-lookup"><span data-stu-id="c5f31-130">type</span></span>|<span data-ttu-id="c5f31-131">Строка</span><span class="sxs-lookup"><span data-stu-id="c5f31-131">String</span></span>|<span data-ttu-id="c5f31-132">Тип учетных данных ключа; например, "Symmetric".</span><span class="sxs-lookup"><span data-stu-id="c5f31-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c5f31-133">usage</span><span class="sxs-lookup"><span data-stu-id="c5f31-133">usage</span></span>|<span data-ttu-id="c5f31-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5f31-134">String</span></span>|<span data-ttu-id="c5f31-135">Строка, описывая назначение, для которого можно использовать ключ; например, "Verify".</span><span class="sxs-lookup"><span data-stu-id="c5f31-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c5f31-136">key</span><span class="sxs-lookup"><span data-stu-id="c5f31-136">key</span></span>|<span data-ttu-id="c5f31-137">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c5f31-137">Binary</span></span>| <span data-ttu-id="c5f31-138">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="c5f31-138">Value for the key credential.</span></span> <span data-ttu-id="c5f31-139">Должно быть значением в коде base 64.</span><span class="sxs-lookup"><span data-stu-id="c5f31-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5f31-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5f31-140">JSON representation</span></span>

<span data-ttu-id="c5f31-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5f31-141">Here is a JSON representation of the resource</span></span>

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


