---
title: Тип ресурса keyCredential
description: Содержит основные учетных данных, связанных с приложением или участников-служб. Свойство **keyCredentials** сущности, приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
ms.openlocfilehash: 0319568dad271f13b396d2f75a71839e85c96c40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851564"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="9e413-104">Тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="9e413-104">keyCredential resource type</span></span>

> <span data-ttu-id="9e413-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e413-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e413-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e413-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e413-107">Содержит основные учетных данных, связанных с приложением или участников-служб.</span><span class="sxs-lookup"><span data-stu-id="9e413-107">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="9e413-108">Свойство **keyCredentials** сущности, [приложения](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="9e413-108">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9e413-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e413-109">JSON representation</span></span>

<span data-ttu-id="9e413-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9e413-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9e413-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e413-111">Properties</span></span>
| <span data-ttu-id="9e413-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e413-112">Property</span></span>     | <span data-ttu-id="9e413-113">Тип</span><span class="sxs-lookup"><span data-stu-id="9e413-113">Type</span></span>   |<span data-ttu-id="9e413-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9e413-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e413-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e413-115">customKeyIdentifier</span></span>|<span data-ttu-id="9e413-116">Binary</span><span class="sxs-lookup"><span data-stu-id="9e413-116">Binary</span></span>| <span data-ttu-id="9e413-117">Настраиваемые идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="9e413-117">Custom key identifier</span></span> |
|<span data-ttu-id="9e413-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9e413-118">endDateTime</span></span>|<span data-ttu-id="9e413-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e413-119">DateTimeOffset</span></span>|<span data-ttu-id="9e413-120">Дата и время истечения срока действия учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9e413-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e413-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9e413-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e413-122">Идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="9e413-122">keyId</span></span>|<span data-ttu-id="9e413-123">Guid</span><span class="sxs-lookup"><span data-stu-id="9e413-123">Guid</span></span>|<span data-ttu-id="9e413-124">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="9e413-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="9e413-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e413-125">startDateTime</span></span>|<span data-ttu-id="9e413-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e413-126">DateTimeOffset</span></span>|<span data-ttu-id="9e413-127">Дата и время, в которой действителен учетных данных. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9e413-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e413-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9e413-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e413-129">type</span><span class="sxs-lookup"><span data-stu-id="9e413-129">type</span></span>|<span data-ttu-id="9e413-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9e413-130">String</span></span>|<span data-ttu-id="9e413-131">Тип ключа учетных данных; Например, «Симметричные».</span><span class="sxs-lookup"><span data-stu-id="9e413-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="9e413-132">об использовании</span><span class="sxs-lookup"><span data-stu-id="9e413-132">usage</span></span>|<span data-ttu-id="9e413-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9e413-133">String</span></span>|<span data-ttu-id="9e413-134">Строка, описывающая назначение, для которого можно использовать ключ; например «проверка».</span><span class="sxs-lookup"><span data-stu-id="9e413-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="9e413-135">key</span><span class="sxs-lookup"><span data-stu-id="9e413-135">key</span></span>|<span data-ttu-id="9e413-136">Двоичный</span><span class="sxs-lookup"><span data-stu-id="9e413-136">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
