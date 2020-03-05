---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 507ea4283ae34e0148d84cd8f76036880a255e98
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523032"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="06ef2-104">Тип ресурса Кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="06ef2-104">keyCredential resource type</span></span>

<span data-ttu-id="06ef2-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06ef2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06ef2-106">Содержит ключевые учетные данные, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="06ef2-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="06ef2-107">Свойство **keyCredentials** сущностей [Application](application.md) и [servicePrincipal](serviceprincipal.md) является коллекцией **кэйкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="06ef2-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="06ef2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="06ef2-108">Properties</span></span>
| <span data-ttu-id="06ef2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="06ef2-109">Property</span></span>     | <span data-ttu-id="06ef2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="06ef2-110">Type</span></span>   |<span data-ttu-id="06ef2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="06ef2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06ef2-112">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="06ef2-112">customKeyIdentifier</span></span>|<span data-ttu-id="06ef2-113">Binary</span><span class="sxs-lookup"><span data-stu-id="06ef2-113">Binary</span></span>| <span data-ttu-id="06ef2-114">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="06ef2-114">Custom key identifier</span></span> |
| <span data-ttu-id="06ef2-115">displayName</span><span class="sxs-lookup"><span data-stu-id="06ef2-115">displayName</span></span> | <span data-ttu-id="06ef2-116">Строка</span><span class="sxs-lookup"><span data-stu-id="06ef2-116">String</span></span> | <span data-ttu-id="06ef2-117">Понятное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="06ef2-117">Friendly name for the key.</span></span> <span data-ttu-id="06ef2-118">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="06ef2-118">Optional.</span></span> |
|<span data-ttu-id="06ef2-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="06ef2-119">endDateTime</span></span>|<span data-ttu-id="06ef2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ef2-120">DateTimeOffset</span></span>|<span data-ttu-id="06ef2-121">Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="06ef2-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06ef2-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="06ef2-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="06ef2-123">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="06ef2-123">keyId</span></span>|<span data-ttu-id="06ef2-124">GUID</span><span class="sxs-lookup"><span data-stu-id="06ef2-124">Guid</span></span>|<span data-ttu-id="06ef2-125">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="06ef2-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="06ef2-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06ef2-126">startDateTime</span></span>|<span data-ttu-id="06ef2-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06ef2-127">DateTimeOffset</span></span>|<span data-ttu-id="06ef2-128">Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="06ef2-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06ef2-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="06ef2-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="06ef2-130">type</span><span class="sxs-lookup"><span data-stu-id="06ef2-130">type</span></span>|<span data-ttu-id="06ef2-131">String</span><span class="sxs-lookup"><span data-stu-id="06ef2-131">String</span></span>|<span data-ttu-id="06ef2-132">Тип учетных данных ключа; Например, "симметричный".</span><span class="sxs-lookup"><span data-stu-id="06ef2-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="06ef2-133">сведений</span><span class="sxs-lookup"><span data-stu-id="06ef2-133">usage</span></span>|<span data-ttu-id="06ef2-134">String</span><span class="sxs-lookup"><span data-stu-id="06ef2-134">String</span></span>|<span data-ttu-id="06ef2-135">Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".</span><span class="sxs-lookup"><span data-stu-id="06ef2-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="06ef2-136">key</span><span class="sxs-lookup"><span data-stu-id="06ef2-136">key</span></span>|<span data-ttu-id="06ef2-137">Двоичный</span><span class="sxs-lookup"><span data-stu-id="06ef2-137">Binary</span></span>| <span data-ttu-id="06ef2-138">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="06ef2-138">Value for the key credential.</span></span> <span data-ttu-id="06ef2-139">Должно быть значением в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="06ef2-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06ef2-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06ef2-140">JSON representation</span></span>

<span data-ttu-id="06ef2-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06ef2-141">Here is a JSON representation of the resource</span></span>

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
