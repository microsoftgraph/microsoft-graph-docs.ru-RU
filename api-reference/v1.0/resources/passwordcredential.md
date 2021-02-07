---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароля, связанные с приложением или основным приложением-службой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d3b180e269b7bd7d16e910d59126c04168ba37a6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136979"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="a9560-103">Тип ресурса passwordCredential</span><span class="sxs-lookup"><span data-stu-id="a9560-103">passwordCredential resource type</span></span>

<span data-ttu-id="a9560-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9560-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9560-105">Представляет учетные данные пароля, связанные с приложением или основным приложением-службой.</span><span class="sxs-lookup"><span data-stu-id="a9560-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="a9560-106">Свойство **passwordCredentials** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="a9560-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="a9560-107">объект — это коллекция объектов **passwordCredential.**</span><span class="sxs-lookup"><span data-stu-id="a9560-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9560-108">Использование POST или PATCH для применения **passwordCredential** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9560-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="a9560-109">Используйте методы addPassword и removePassword для обновления пароля приложения или servicePrincipal:</span><span class="sxs-lookup"><span data-stu-id="a9560-109">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="a9560-110">application: addPassword</span><span class="sxs-lookup"><span data-stu-id="a9560-110">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="a9560-111">application: removePassword</span><span class="sxs-lookup"><span data-stu-id="a9560-111">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="a9560-112">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="a9560-112">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="a9560-113">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="a9560-113">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a><span data-ttu-id="a9560-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9560-114">Properties</span></span>
| <span data-ttu-id="a9560-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9560-115">Property</span></span>     | <span data-ttu-id="a9560-116">Тип</span><span class="sxs-lookup"><span data-stu-id="a9560-116">Type</span></span>   |<span data-ttu-id="a9560-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a9560-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9560-118">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="a9560-118">customKeyIdentifier</span></span> | <span data-ttu-id="a9560-119">Binary</span><span class="sxs-lookup"><span data-stu-id="a9560-119">Binary</span></span> | <span data-ttu-id="a9560-120">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="a9560-120">Do not use.</span></span> |
| <span data-ttu-id="a9560-121">displayName</span><span class="sxs-lookup"><span data-stu-id="a9560-121">displayName</span></span> | <span data-ttu-id="a9560-122">String</span><span class="sxs-lookup"><span data-stu-id="a9560-122">String</span></span> | <span data-ttu-id="a9560-123">Удобное имя пароля.</span><span class="sxs-lookup"><span data-stu-id="a9560-123">Friendly name for the password.</span></span> <span data-ttu-id="a9560-124">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9560-124">Optional.</span></span> |
| <span data-ttu-id="a9560-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a9560-125">endDateTime</span></span> | <span data-ttu-id="a9560-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9560-126">DateTimeOffset</span></span> | <span data-ttu-id="a9560-127">Дата и время истечения срока действия пароля представлены в формате ISO 8601 и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a9560-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a9560-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9560-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a9560-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9560-129">Optional.</span></span> |
| <span data-ttu-id="a9560-130">hint</span><span class="sxs-lookup"><span data-stu-id="a9560-130">hint</span></span> | <span data-ttu-id="a9560-131">String</span><span class="sxs-lookup"><span data-stu-id="a9560-131">String</span></span> | <span data-ttu-id="a9560-132">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="a9560-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="a9560-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9560-133">Read-only.</span></span> |
| <span data-ttu-id="a9560-134">keyId</span><span class="sxs-lookup"><span data-stu-id="a9560-134">keyId</span></span> | <span data-ttu-id="a9560-135">Guid</span><span class="sxs-lookup"><span data-stu-id="a9560-135">Guid</span></span> | <span data-ttu-id="a9560-136">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="a9560-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="a9560-137">secretText</span><span class="sxs-lookup"><span data-stu-id="a9560-137">secretText</span></span> | <span data-ttu-id="a9560-138">String</span><span class="sxs-lookup"><span data-stu-id="a9560-138">String</span></span> | <span data-ttu-id="a9560-139">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16–64 символа.</span><span class="sxs-lookup"><span data-stu-id="a9560-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="a9560-140">Созданный пароль возвращается только во время первоначального запроса POST для [addPassword.](../api/application-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="a9560-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="a9560-141">В будущем получить этот пароль будет не нужно.</span><span class="sxs-lookup"><span data-stu-id="a9560-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="a9560-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a9560-142">startDateTime</span></span> | <span data-ttu-id="a9560-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9560-143">DateTimeOffset</span></span> | <span data-ttu-id="a9560-144">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="a9560-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="a9560-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a9560-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a9560-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9560-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a9560-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a9560-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="a9560-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9560-148">JSON representation</span></span>

<span data-ttu-id="a9560-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9560-149">The following is a JSON representation of the resource.</span></span>

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

