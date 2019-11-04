---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 346ff30ad0479d2b25dc57d09a67cc4ddd5f83bc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939630"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c55fc-104">Тип ресурса Кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="c55fc-104">keyCredential resource type</span></span>

<span data-ttu-id="c55fc-105">Содержит ключевые учетные данные, связанные с приложением</span><span class="sxs-lookup"><span data-stu-id="c55fc-105">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="c55fc-106">.</span><span class="sxs-lookup"><span data-stu-id="c55fc-106"></span></span> <span data-ttu-id="c55fc-107">Свойство **keyCredentials** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="c55fc-107">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="c55fc-108">сущность представляет собой коллекцию **кэйкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="c55fc-108">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="c55fc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c55fc-109">Properties</span></span>
| <span data-ttu-id="c55fc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c55fc-110">Property</span></span>     | <span data-ttu-id="c55fc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c55fc-111">Type</span></span>   |<span data-ttu-id="c55fc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c55fc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c55fc-113">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="c55fc-113">customKeyIdentifier</span></span>|<span data-ttu-id="c55fc-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c55fc-114">Binary</span></span>| <span data-ttu-id="c55fc-115">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="c55fc-115">Custom key identifier</span></span> |
| <span data-ttu-id="c55fc-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c55fc-116">displayName</span></span> | <span data-ttu-id="c55fc-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c55fc-117">String</span></span> | <span data-ttu-id="c55fc-118">Понятное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="c55fc-118">Friendly name for the key.</span></span> <span data-ttu-id="c55fc-119">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c55fc-119">Optional.</span></span> |
|<span data-ttu-id="c55fc-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c55fc-120">endDateTime</span></span>|<span data-ttu-id="c55fc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c55fc-121">DateTimeOffset</span></span>|<span data-ttu-id="c55fc-122">Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c55fc-122">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c55fc-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c55fc-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c55fc-124">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="c55fc-124">keyId</span></span>|<span data-ttu-id="c55fc-125">GUID</span><span class="sxs-lookup"><span data-stu-id="c55fc-125">Guid</span></span>|<span data-ttu-id="c55fc-126">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="c55fc-126">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c55fc-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c55fc-127">startDateTime</span></span>|<span data-ttu-id="c55fc-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c55fc-128">DateTimeOffset</span></span>|<span data-ttu-id="c55fc-129">Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c55fc-129">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c55fc-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c55fc-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c55fc-131">type</span><span class="sxs-lookup"><span data-stu-id="c55fc-131">type</span></span>|<span data-ttu-id="c55fc-132">String</span><span class="sxs-lookup"><span data-stu-id="c55fc-132">String</span></span>|<span data-ttu-id="c55fc-133">Тип учетных данных ключа; Например, "симметричный".</span><span class="sxs-lookup"><span data-stu-id="c55fc-133">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c55fc-134">сведений</span><span class="sxs-lookup"><span data-stu-id="c55fc-134">usage</span></span>|<span data-ttu-id="c55fc-135">String</span><span class="sxs-lookup"><span data-stu-id="c55fc-135">String</span></span>|<span data-ttu-id="c55fc-136">Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".</span><span class="sxs-lookup"><span data-stu-id="c55fc-136">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c55fc-137">key</span><span class="sxs-lookup"><span data-stu-id="c55fc-137">key</span></span>|<span data-ttu-id="c55fc-138">Двоичный</span><span class="sxs-lookup"><span data-stu-id="c55fc-138">Binary</span></span>| <span data-ttu-id="c55fc-139">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="c55fc-139">Value for the key credential.</span></span> <span data-ttu-id="c55fc-140">Должно быть значением в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="c55fc-140">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c55fc-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c55fc-141">JSON representation</span></span>

<span data-ttu-id="c55fc-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c55fc-142">Here is a JSON representation of the resource</span></span>

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
