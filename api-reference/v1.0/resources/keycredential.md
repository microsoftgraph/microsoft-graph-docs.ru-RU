---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 97aab57c1ed0aa9f43536b89b49ca93a422962da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072937"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="81a99-104">Тип ресурса Кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="81a99-104">keyCredential resource type</span></span>

<span data-ttu-id="81a99-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a99-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81a99-106">Содержит ключевые учетные данные, связанные с приложением</span><span class="sxs-lookup"><span data-stu-id="81a99-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="81a99-107">.</span><span class="sxs-lookup"><span data-stu-id="81a99-107">.</span></span> <span data-ttu-id="81a99-108">Свойство **keyCredentials** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="81a99-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="81a99-109">сущность представляет собой коллекцию **кэйкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="81a99-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="81a99-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="81a99-110">Properties</span></span>
| <span data-ttu-id="81a99-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="81a99-111">Property</span></span>     | <span data-ttu-id="81a99-112">Тип</span><span class="sxs-lookup"><span data-stu-id="81a99-112">Type</span></span>   |<span data-ttu-id="81a99-113">Описание</span><span class="sxs-lookup"><span data-stu-id="81a99-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a99-114">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="81a99-114">customKeyIdentifier</span></span>|<span data-ttu-id="81a99-115">Binary</span><span class="sxs-lookup"><span data-stu-id="81a99-115">Binary</span></span>| <span data-ttu-id="81a99-116">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="81a99-116">Custom key identifier</span></span> |
| <span data-ttu-id="81a99-117">displayName</span><span class="sxs-lookup"><span data-stu-id="81a99-117">displayName</span></span> | <span data-ttu-id="81a99-118">Строка</span><span class="sxs-lookup"><span data-stu-id="81a99-118">String</span></span> | <span data-ttu-id="81a99-119">Понятное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="81a99-119">Friendly name for the key.</span></span> <span data-ttu-id="81a99-120">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="81a99-120">Optional.</span></span> |
|<span data-ttu-id="81a99-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="81a99-121">endDateTime</span></span>|<span data-ttu-id="81a99-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a99-122">DateTimeOffset</span></span>|<span data-ttu-id="81a99-123">Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81a99-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81a99-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="81a99-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="81a99-125">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="81a99-125">keyId</span></span>|<span data-ttu-id="81a99-126">Guid</span><span class="sxs-lookup"><span data-stu-id="81a99-126">Guid</span></span>|<span data-ttu-id="81a99-127">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="81a99-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="81a99-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81a99-128">startDateTime</span></span>|<span data-ttu-id="81a99-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a99-129">DateTimeOffset</span></span>|<span data-ttu-id="81a99-130">Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="81a99-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="81a99-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="81a99-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="81a99-132">type</span><span class="sxs-lookup"><span data-stu-id="81a99-132">type</span></span>|<span data-ttu-id="81a99-133">Строка</span><span class="sxs-lookup"><span data-stu-id="81a99-133">String</span></span>|<span data-ttu-id="81a99-134">Тип учетных данных ключа; Например, "симметричный".</span><span class="sxs-lookup"><span data-stu-id="81a99-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="81a99-135">сведений</span><span class="sxs-lookup"><span data-stu-id="81a99-135">usage</span></span>|<span data-ttu-id="81a99-136">Строка</span><span class="sxs-lookup"><span data-stu-id="81a99-136">String</span></span>|<span data-ttu-id="81a99-137">Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".</span><span class="sxs-lookup"><span data-stu-id="81a99-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="81a99-138">key</span><span class="sxs-lookup"><span data-stu-id="81a99-138">key</span></span>|<span data-ttu-id="81a99-139">Двоичный</span><span class="sxs-lookup"><span data-stu-id="81a99-139">Binary</span></span>| <span data-ttu-id="81a99-140">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="81a99-140">Value for the key credential.</span></span> <span data-ttu-id="81a99-141">Должно быть значением в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="81a99-141">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81a99-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81a99-142">JSON representation</span></span>

<span data-ttu-id="81a99-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81a99-143">Here is a JSON representation of the resource</span></span>

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

