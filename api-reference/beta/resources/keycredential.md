---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 57305e7e5767b8ad5454d7fd3a229be53489b5fd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939259"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="8b399-104">Тип ресурса Кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="8b399-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b399-105">Содержит ключевые учетные данные, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="8b399-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="8b399-106">Свойство **keyCredentials** сущностей [Application](application.md) и [servicePrincipal](serviceprincipal.md) является коллекцией **кэйкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="8b399-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="8b399-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b399-107">Properties</span></span>
| <span data-ttu-id="8b399-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b399-108">Property</span></span>     | <span data-ttu-id="8b399-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b399-109">Type</span></span>   |<span data-ttu-id="8b399-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b399-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b399-111">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="8b399-111">customKeyIdentifier</span></span>|<span data-ttu-id="8b399-112">Binary</span><span class="sxs-lookup"><span data-stu-id="8b399-112">Binary</span></span>| <span data-ttu-id="8b399-113">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="8b399-113">Custom key identifier</span></span> |
| <span data-ttu-id="8b399-114">displayName</span><span class="sxs-lookup"><span data-stu-id="8b399-114">displayName</span></span> | <span data-ttu-id="8b399-115">Строка</span><span class="sxs-lookup"><span data-stu-id="8b399-115">String</span></span> | <span data-ttu-id="8b399-116">Понятное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="8b399-116">Friendly name for the key.</span></span> <span data-ttu-id="8b399-117">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="8b399-117">Optional.</span></span> |
|<span data-ttu-id="8b399-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8b399-118">endDateTime</span></span>|<span data-ttu-id="8b399-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b399-119">DateTimeOffset</span></span>|<span data-ttu-id="8b399-120">Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8b399-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8b399-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8b399-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8b399-122">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="8b399-122">keyId</span></span>|<span data-ttu-id="8b399-123">GUID</span><span class="sxs-lookup"><span data-stu-id="8b399-123">Guid</span></span>|<span data-ttu-id="8b399-124">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="8b399-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="8b399-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8b399-125">startDateTime</span></span>|<span data-ttu-id="8b399-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b399-126">DateTimeOffset</span></span>|<span data-ttu-id="8b399-127">Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8b399-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8b399-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8b399-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8b399-129">type</span><span class="sxs-lookup"><span data-stu-id="8b399-129">type</span></span>|<span data-ttu-id="8b399-130">String</span><span class="sxs-lookup"><span data-stu-id="8b399-130">String</span></span>|<span data-ttu-id="8b399-131">Тип учетных данных ключа; Например, "симметричный".</span><span class="sxs-lookup"><span data-stu-id="8b399-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="8b399-132">сведений</span><span class="sxs-lookup"><span data-stu-id="8b399-132">usage</span></span>|<span data-ttu-id="8b399-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8b399-133">String</span></span>|<span data-ttu-id="8b399-134">Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".</span><span class="sxs-lookup"><span data-stu-id="8b399-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="8b399-135">key</span><span class="sxs-lookup"><span data-stu-id="8b399-135">key</span></span>|<span data-ttu-id="8b399-136">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8b399-136">Binary</span></span>| <span data-ttu-id="8b399-137">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="8b399-137">Value for the key credential.</span></span> <span data-ttu-id="8b399-138">Должно быть значением в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="8b399-138">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b399-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b399-139">JSON representation</span></span>

<span data-ttu-id="8b399-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b399-140">Here is a JSON representation of the resource</span></span>

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
