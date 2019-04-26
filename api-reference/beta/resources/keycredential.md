---
title: Тип ресурса Кэйкредентиал
description: Содержит ключевые учетные данные, связанные с приложением или субъектом службы. Свойство **keyCredentials** сущностей Application и servicePrincipal является коллекцией **кэйкредентиал**.
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562673"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="9a3a0-104">Тип ресурса Кэйкредентиал</span><span class="sxs-lookup"><span data-stu-id="9a3a0-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a3a0-105">Содержит ключевые учетные данные, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="9a3a0-106">Свойство **keyCredentials** сущностей [Application](application.md) и [servicePrincipal](serviceprincipal.md) является коллекцией **кэйкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9a3a0-107">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9a3a0-107">JSON representation</span></span>

<span data-ttu-id="9a3a0-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9a3a0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a3a0-109">Properties</span></span>
| <span data-ttu-id="9a3a0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a3a0-110">Property</span></span>     | <span data-ttu-id="9a3a0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9a3a0-111">Type</span></span>   |<span data-ttu-id="9a3a0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9a3a0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a3a0-113">Кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="9a3a0-113">customKeyIdentifier</span></span>|<span data-ttu-id="9a3a0-114">Двоичный</span><span class="sxs-lookup"><span data-stu-id="9a3a0-114">Binary</span></span>| <span data-ttu-id="9a3a0-115">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="9a3a0-115">Custom key identifier</span></span> |
|<span data-ttu-id="9a3a0-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9a3a0-116">endDateTime</span></span>|<span data-ttu-id="9a3a0-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a3a0-117">DateTimeOffset</span></span>|<span data-ttu-id="9a3a0-118">Дата и время истечения срока действия учетных данных. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a3a0-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a3a0-120">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="9a3a0-120">keyId</span></span>|<span data-ttu-id="9a3a0-121">Guid</span><span class="sxs-lookup"><span data-stu-id="9a3a0-121">Guid</span></span>|<span data-ttu-id="9a3a0-122">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="9a3a0-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a3a0-123">startDateTime</span></span>|<span data-ttu-id="9a3a0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a3a0-124">DateTimeOffset</span></span>|<span data-ttu-id="9a3a0-125">Дата и время, когда учетные данные становятся действительными. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a3a0-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9a3a0-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a3a0-127">type</span><span class="sxs-lookup"><span data-stu-id="9a3a0-127">type</span></span>|<span data-ttu-id="9a3a0-128">String</span><span class="sxs-lookup"><span data-stu-id="9a3a0-128">String</span></span>|<span data-ttu-id="9a3a0-129">Тип учетных данных ключа; Например, "симметричный".</span><span class="sxs-lookup"><span data-stu-id="9a3a0-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="9a3a0-130">сведений</span><span class="sxs-lookup"><span data-stu-id="9a3a0-130">usage</span></span>|<span data-ttu-id="9a3a0-131">String</span><span class="sxs-lookup"><span data-stu-id="9a3a0-131">String</span></span>|<span data-ttu-id="9a3a0-132">Строка, описывающая цель, для которой можно использовать ключ; Пример: "Verify".</span><span class="sxs-lookup"><span data-stu-id="9a3a0-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="9a3a0-133">key</span><span class="sxs-lookup"><span data-stu-id="9a3a0-133">key</span></span>|<span data-ttu-id="9a3a0-134">Двоичный</span><span class="sxs-lookup"><span data-stu-id="9a3a0-134">Binary</span></span>|            |

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
