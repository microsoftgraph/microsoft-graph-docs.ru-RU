---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы. Свойство **пассвордкредентиалс** объекта servicePrincipal и сущности приложения является коллекцией **пассвордкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 5cdb9543bed0cecf50428dc3461d4909977325dd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934255"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="3960c-104">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="3960c-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3960c-105">Представляет учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="3960c-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="3960c-106">Свойство **пассвордкредентиалс** [приложения](application.md) и [servicePrincipal](serviceprincipal.md) ентититес — это коллекция объектов **пассвордкредентиал** .</span><span class="sxs-lookup"><span data-stu-id="3960c-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> <span data-ttu-id="3960c-107">Note: использование PATCH для обновления Пассвордкредентиалс не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3960c-107">Note: Using PATCH to update passwordCredentials is not supported.</span></span> <span data-ttu-id="3960c-108">Используйте методы Аддпассворд и Ремовепассворд для обновления пароля приложения или servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="3960c-108">Use use the addPassword and removePassword methods to update the password for an application or a servicePrincipal.</span></span>
>
> - <span data-ttu-id="3960c-109">Application — [аддпассворд](../api/application-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="3960c-109">application - [addPassword](../api/application-addpassword.md)</span></span>
> - <span data-ttu-id="3960c-110">Application — [ремовепассворд](../api/application-removepassword.md)</span><span class="sxs-lookup"><span data-stu-id="3960c-110">application - [removePassword](../api/application-removepassword.md)</span></span>
> - <span data-ttu-id="3960c-111">servicePrincipal — [аддпассворд](../api/serviceprincipal-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="3960c-111">servicePrincipal - [addPassword](../api/serviceprincipal-addpassword.md)</span></span>
> - <span data-ttu-id="3960c-112">servicePrincipal — [ремовепассворд](../api/serviceprincipal-removepassword.md)</span><span class="sxs-lookup"><span data-stu-id="3960c-112">servicePrincipal - [removePassword](../api/serviceprincipal-removepassword.md)</span></span>


## <a name="properties"></a><span data-ttu-id="3960c-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="3960c-113">Properties</span></span>
| <span data-ttu-id="3960c-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="3960c-114">Property</span></span>     | <span data-ttu-id="3960c-115">Тип</span><span class="sxs-lookup"><span data-stu-id="3960c-115">Type</span></span>   |<span data-ttu-id="3960c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="3960c-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3960c-117">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="3960c-117">customKeyIdentifier</span></span> | <span data-ttu-id="3960c-118">Binary</span><span class="sxs-lookup"><span data-stu-id="3960c-118">Binary</span></span> | <span data-ttu-id="3960c-119">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="3960c-119">Do not use.</span></span> |
| <span data-ttu-id="3960c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="3960c-120">displayName</span></span> | <span data-ttu-id="3960c-121">Строка</span><span class="sxs-lookup"><span data-stu-id="3960c-121">String</span></span> | <span data-ttu-id="3960c-122">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="3960c-122">Friendly name for the password.</span></span> <span data-ttu-id="3960c-123">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="3960c-123">Optional.</span></span> |
| <span data-ttu-id="3960c-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3960c-124">endDateTime</span></span> | <span data-ttu-id="3960c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3960c-125">DateTimeOffset</span></span> | <span data-ttu-id="3960c-126">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3960c-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3960c-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3960c-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3960c-128">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="3960c-128">Optional.</span></span> |
| <span data-ttu-id="3960c-129">сказок</span><span class="sxs-lookup"><span data-stu-id="3960c-129">hint</span></span> | <span data-ttu-id="3960c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="3960c-130">String</span></span> | <span data-ttu-id="3960c-131">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="3960c-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="3960c-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3960c-132">Read-only.</span></span> |
| <span data-ttu-id="3960c-133">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="3960c-133">keyId</span></span> | <span data-ttu-id="3960c-134">GUID</span><span class="sxs-lookup"><span data-stu-id="3960c-134">Guid</span></span> | <span data-ttu-id="3960c-135">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="3960c-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="3960c-136">секреттекст</span><span class="sxs-lookup"><span data-stu-id="3960c-136">secretText</span></span> | <span data-ttu-id="3960c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3960c-137">String</span></span> | <span data-ttu-id="3960c-138">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="3960c-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="3960c-139">Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="3960c-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="3960c-140">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="3960c-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="3960c-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3960c-141">startDateTime</span></span> | <span data-ttu-id="3960c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3960c-142">DateTimeOffset</span></span> | <span data-ttu-id="3960c-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="3960c-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="3960c-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3960c-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3960c-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3960c-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3960c-146">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="3960c-146">Optional.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a><span data-ttu-id="3960c-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3960c-147">JSON representation</span></span>

<span data-ttu-id="3960c-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3960c-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "Guid",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
