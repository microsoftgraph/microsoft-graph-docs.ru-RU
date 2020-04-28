---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 82017d36521bcb03364ab097863cbcaf70ccf3bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447935"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="4bcbc-103">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="4bcbc-103">passwordCredential resource type</span></span>

<span data-ttu-id="4bcbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bcbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bcbc-105">Представляет учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="4bcbc-106">Свойство **пассвордкредентиалс** [приложения](application.md) и [servicePrincipal](serviceprincipal.md) ентититес — это коллекция объектов **пассвордкредентиал** .</span><span class="sxs-lookup"><span data-stu-id="4bcbc-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4bcbc-107">Использование POST или PATCH для установки **пассвордкредентиал** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-107">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="4bcbc-108">Используйте методы Аддпассворд и Ремовепассворд для обновления пароля приложения или servicePrincipal:</span><span class="sxs-lookup"><span data-stu-id="4bcbc-108">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="4bcbc-109">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="4bcbc-109">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="4bcbc-110">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="4bcbc-110">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="4bcbc-111">servicePrincipal: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="4bcbc-111">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="4bcbc-112">servicePrincipal: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="4bcbc-112">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a><span data-ttu-id="4bcbc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bcbc-113">Properties</span></span>
| <span data-ttu-id="4bcbc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bcbc-114">Property</span></span>     | <span data-ttu-id="4bcbc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4bcbc-115">Type</span></span>   |<span data-ttu-id="4bcbc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4bcbc-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bcbc-117">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="4bcbc-117">customKeyIdentifier</span></span> | <span data-ttu-id="4bcbc-118">Binary</span><span class="sxs-lookup"><span data-stu-id="4bcbc-118">Binary</span></span> | <span data-ttu-id="4bcbc-119">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-119">Do not use.</span></span> |
| <span data-ttu-id="4bcbc-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4bcbc-120">displayName</span></span> | <span data-ttu-id="4bcbc-121">String</span><span class="sxs-lookup"><span data-stu-id="4bcbc-121">String</span></span> | <span data-ttu-id="4bcbc-122">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-122">Friendly name for the password.</span></span> <span data-ttu-id="4bcbc-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-123">Optional.</span></span> |
| <span data-ttu-id="4bcbc-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4bcbc-124">endDateTime</span></span> | <span data-ttu-id="4bcbc-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bcbc-125">DateTimeOffset</span></span> | <span data-ttu-id="4bcbc-126">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4bcbc-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4bcbc-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-128">Optional.</span></span> |
| <span data-ttu-id="4bcbc-129">сказок</span><span class="sxs-lookup"><span data-stu-id="4bcbc-129">hint</span></span> | <span data-ttu-id="4bcbc-130">String</span><span class="sxs-lookup"><span data-stu-id="4bcbc-130">String</span></span> | <span data-ttu-id="4bcbc-131">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="4bcbc-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-132">Read-only.</span></span> |
| <span data-ttu-id="4bcbc-133">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="4bcbc-133">keyId</span></span> | <span data-ttu-id="4bcbc-134">GUID</span><span class="sxs-lookup"><span data-stu-id="4bcbc-134">Guid</span></span> | <span data-ttu-id="4bcbc-135">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="4bcbc-136">секреттекст</span><span class="sxs-lookup"><span data-stu-id="4bcbc-136">secretText</span></span> | <span data-ttu-id="4bcbc-137">String</span><span class="sxs-lookup"><span data-stu-id="4bcbc-137">String</span></span> | <span data-ttu-id="4bcbc-138">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="4bcbc-139">Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="4bcbc-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="4bcbc-140">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="4bcbc-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4bcbc-141">startDateTime</span></span> | <span data-ttu-id="4bcbc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4bcbc-142">DateTimeOffset</span></span> | <span data-ttu-id="4bcbc-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="4bcbc-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4bcbc-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4bcbc-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4bcbc-146">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="4bcbc-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bcbc-147">JSON representation</span></span>

<span data-ttu-id="4bcbc-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bcbc-148">The following is a JSON representation of the resource.</span></span>

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
