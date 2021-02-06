---
title: Тип ресурса passwordCredential
description: Содержит учетные данные пароля, связанные с приложением или основным приложением-службой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6f7906f2f7411c680eb07c94166e5d324e922d67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137664"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="188fb-103">Тип ресурса passwordCredential</span><span class="sxs-lookup"><span data-stu-id="188fb-103">passwordCredential resource type</span></span>

<span data-ttu-id="188fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="188fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="188fb-105">Представляет учетные данные пароля, связанные с приложением или основным приложением-службой.</span><span class="sxs-lookup"><span data-stu-id="188fb-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="188fb-106">Свойство **passwordCredentials** объектов [application](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **объектов passwordCredential.**</span><span class="sxs-lookup"><span data-stu-id="188fb-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="188fb-107">Использование POST или PATCH для применения **passwordCredential** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="188fb-107">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="188fb-108">Используйте методы addPassword и removePassword для обновления пароля приложения или servicePrincipal:</span><span class="sxs-lookup"><span data-stu-id="188fb-108">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="188fb-109">application: addPassword</span><span class="sxs-lookup"><span data-stu-id="188fb-109">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="188fb-110">application: removePassword</span><span class="sxs-lookup"><span data-stu-id="188fb-110">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="188fb-111">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="188fb-111">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="188fb-112">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="188fb-112">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a><span data-ttu-id="188fb-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="188fb-113">Properties</span></span>
| <span data-ttu-id="188fb-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="188fb-114">Property</span></span>     | <span data-ttu-id="188fb-115">Тип</span><span class="sxs-lookup"><span data-stu-id="188fb-115">Type</span></span>   |<span data-ttu-id="188fb-116">Описание</span><span class="sxs-lookup"><span data-stu-id="188fb-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="188fb-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="188fb-117">customKeyIdentifier</span></span> | <span data-ttu-id="188fb-118">Binary</span><span class="sxs-lookup"><span data-stu-id="188fb-118">Binary</span></span> | <span data-ttu-id="188fb-119">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="188fb-119">Do not use.</span></span> |
| <span data-ttu-id="188fb-120">displayName</span><span class="sxs-lookup"><span data-stu-id="188fb-120">displayName</span></span> | <span data-ttu-id="188fb-121">Строка</span><span class="sxs-lookup"><span data-stu-id="188fb-121">String</span></span> | <span data-ttu-id="188fb-122">Удобное имя пароля.</span><span class="sxs-lookup"><span data-stu-id="188fb-122">Friendly name for the password.</span></span> <span data-ttu-id="188fb-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="188fb-123">Optional.</span></span> |
| <span data-ttu-id="188fb-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="188fb-124">endDateTime</span></span> | <span data-ttu-id="188fb-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="188fb-125">DateTimeOffset</span></span> | <span data-ttu-id="188fb-126">Дата и время истечения срока действия пароля представлены в формате ISO 8601 и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="188fb-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="188fb-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="188fb-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="188fb-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="188fb-128">Optional.</span></span> |
| <span data-ttu-id="188fb-129">hint</span><span class="sxs-lookup"><span data-stu-id="188fb-129">hint</span></span> | <span data-ttu-id="188fb-130">Строка</span><span class="sxs-lookup"><span data-stu-id="188fb-130">String</span></span> | <span data-ttu-id="188fb-131">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="188fb-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="188fb-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="188fb-132">Read-only.</span></span> |
| <span data-ttu-id="188fb-133">keyId</span><span class="sxs-lookup"><span data-stu-id="188fb-133">keyId</span></span> | <span data-ttu-id="188fb-134">Guid</span><span class="sxs-lookup"><span data-stu-id="188fb-134">Guid</span></span> | <span data-ttu-id="188fb-135">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="188fb-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="188fb-136">secretText</span><span class="sxs-lookup"><span data-stu-id="188fb-136">secretText</span></span> | <span data-ttu-id="188fb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="188fb-137">String</span></span> | <span data-ttu-id="188fb-138">Только для чтения; Содержит надежные пароли, созданные в Azure AD длиной от 16 до 64 символов.</span><span class="sxs-lookup"><span data-stu-id="188fb-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="188fb-139">Созданный пароль возвращается только во время первоначального запроса POST для [addPassword.](../api/application-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="188fb-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="188fb-140">В будущем получить этот пароль будет не нужно.</span><span class="sxs-lookup"><span data-stu-id="188fb-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="188fb-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="188fb-141">startDateTime</span></span> | <span data-ttu-id="188fb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="188fb-142">DateTimeOffset</span></span> | <span data-ttu-id="188fb-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="188fb-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="188fb-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="188fb-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="188fb-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="188fb-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="188fb-146">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="188fb-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="188fb-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="188fb-147">JSON representation</span></span>

<span data-ttu-id="188fb-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="188fb-148">The following is a JSON representation of the resource.</span></span>

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


