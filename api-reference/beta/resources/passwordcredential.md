---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароль, связанный с приложением или участника службы. Свойство **passwordCredentials** servicePrincipal сущности и сущности приложения — это коллекция **passwordCredential**.
localization_priority: Normal
ms.openlocfilehash: 5cb995c00a7dcfcfb4bda331e24dcb4d732f04f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814443"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="921bc-104">Тип ресурса passwordCredential</span><span class="sxs-lookup"><span data-stu-id="921bc-104">passwordCredential resource type</span></span>

> <span data-ttu-id="921bc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="921bc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="921bc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="921bc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="921bc-107">Содержит учетные данные пароль, связанный с приложением или участника службы.</span><span class="sxs-lookup"><span data-stu-id="921bc-107">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="921bc-108">Свойство **passwordCredentials** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **passwordCredential**.</span><span class="sxs-lookup"><span data-stu-id="921bc-108">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="921bc-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="921bc-109">JSON representation</span></span>

<span data-ttu-id="921bc-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="921bc-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="921bc-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="921bc-111">Properties</span></span>
| <span data-ttu-id="921bc-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="921bc-112">Property</span></span>     | <span data-ttu-id="921bc-113">Тип</span><span class="sxs-lookup"><span data-stu-id="921bc-113">Type</span></span>   |<span data-ttu-id="921bc-114">Описание</span><span class="sxs-lookup"><span data-stu-id="921bc-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="921bc-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="921bc-115">customKeyIdentifier</span></span>|<span data-ttu-id="921bc-116">Binary</span><span class="sxs-lookup"><span data-stu-id="921bc-116">Binary</span></span>|            |
|<span data-ttu-id="921bc-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="921bc-117">endDateTime</span></span>|<span data-ttu-id="921bc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921bc-118">DateTimeOffset</span></span>|<span data-ttu-id="921bc-119">Дата и время истечения срока действия пароля. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="921bc-119">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="921bc-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="921bc-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="921bc-121">Идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="921bc-121">keyId</span></span>|<span data-ttu-id="921bc-122">Guid</span><span class="sxs-lookup"><span data-stu-id="921bc-122">Guid</span></span>|            |
|<span data-ttu-id="921bc-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="921bc-123">startDateTime</span></span>|<span data-ttu-id="921bc-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="921bc-124">DateTimeOffset</span></span>|<span data-ttu-id="921bc-125">Дата и время, в которой становится допустимый пароль. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="921bc-125">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="921bc-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="921bc-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="921bc-127">secretText</span><span class="sxs-lookup"><span data-stu-id="921bc-127">secretText</span></span>|<span data-ttu-id="921bc-128">Строка</span><span class="sxs-lookup"><span data-stu-id="921bc-128">String</span></span>| <span data-ttu-id="921bc-129">Пароли должны быть 16-64 символов</span><span class="sxs-lookup"><span data-stu-id="921bc-129">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="921bc-130">подсказка</span><span class="sxs-lookup"><span data-stu-id="921bc-130">hint</span></span>|<span data-ttu-id="921bc-131">String</span><span class="sxs-lookup"><span data-stu-id="921bc-131">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
