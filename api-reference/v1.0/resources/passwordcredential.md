---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы. Свойство **пассвордкредентиалс** объекта servicePrincipal и сущности приложения является коллекцией **пассвордкредентиал**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 0067b993cfc7d9708673bf25b20ecc054bff7925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534081"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="320c8-104">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="320c8-104">passwordCredential resource type</span></span>

<span data-ttu-id="320c8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="320c8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="320c8-106">Представляет учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="320c8-106">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="320c8-107">Свойство **пассвордкредентиалс** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="320c8-107">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="320c8-108">сущность — это коллекция объектов **пассвордкредентиал** .</span><span class="sxs-lookup"><span data-stu-id="320c8-108">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="320c8-109">Использование POST или PATCH для установки **пассвордкредентиал** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="320c8-109">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="320c8-110">Использование методов Аддпассворд и Ремовепассворд для обновления пароля приложения</span><span class="sxs-lookup"><span data-stu-id="320c8-110">Use the addPassword and removePassword methods to update the password for an application</span></span><!--or a servicePrincipal--><span data-ttu-id="320c8-111">:</span><span class="sxs-lookup"><span data-stu-id="320c8-111">:</span></span>
>
> - [<span data-ttu-id="320c8-112">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="320c8-112">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="320c8-113">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="320c8-113">application: removePassword</span></span>](../api/application-removepassword.md)
<!--
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a><span data-ttu-id="320c8-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="320c8-114">Properties</span></span>
| <span data-ttu-id="320c8-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="320c8-115">Property</span></span>     | <span data-ttu-id="320c8-116">Тип</span><span class="sxs-lookup"><span data-stu-id="320c8-116">Type</span></span>   |<span data-ttu-id="320c8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="320c8-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="320c8-118">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="320c8-118">customKeyIdentifier</span></span> | <span data-ttu-id="320c8-119">Binary</span><span class="sxs-lookup"><span data-stu-id="320c8-119">Binary</span></span> | <span data-ttu-id="320c8-120">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="320c8-120">Do not use.</span></span> |
| <span data-ttu-id="320c8-121">displayName</span><span class="sxs-lookup"><span data-stu-id="320c8-121">displayName</span></span> | <span data-ttu-id="320c8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="320c8-122">String</span></span> | <span data-ttu-id="320c8-123">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="320c8-123">Friendly name for the password.</span></span> <span data-ttu-id="320c8-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="320c8-124">Optional.</span></span> |
| <span data-ttu-id="320c8-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="320c8-125">endDateTime</span></span> | <span data-ttu-id="320c8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="320c8-126">DateTimeOffset</span></span> | <span data-ttu-id="320c8-127">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="320c8-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="320c8-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="320c8-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="320c8-129">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="320c8-129">Optional.</span></span> |
| <span data-ttu-id="320c8-130">сказок</span><span class="sxs-lookup"><span data-stu-id="320c8-130">hint</span></span> | <span data-ttu-id="320c8-131">Строка</span><span class="sxs-lookup"><span data-stu-id="320c8-131">String</span></span> | <span data-ttu-id="320c8-132">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="320c8-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="320c8-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="320c8-133">Read-only.</span></span> |
| <span data-ttu-id="320c8-134">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="320c8-134">keyId</span></span> | <span data-ttu-id="320c8-135">GUID</span><span class="sxs-lookup"><span data-stu-id="320c8-135">Guid</span></span> | <span data-ttu-id="320c8-136">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="320c8-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="320c8-137">секреттекст</span><span class="sxs-lookup"><span data-stu-id="320c8-137">secretText</span></span> | <span data-ttu-id="320c8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="320c8-138">String</span></span> | <span data-ttu-id="320c8-139">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="320c8-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="320c8-140">Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="320c8-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="320c8-141">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="320c8-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="320c8-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="320c8-142">startDateTime</span></span> | <span data-ttu-id="320c8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="320c8-143">DateTimeOffset</span></span> | <span data-ttu-id="320c8-144">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="320c8-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="320c8-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="320c8-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="320c8-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="320c8-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="320c8-147">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="320c8-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="320c8-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="320c8-148">JSON representation</span></span>

<span data-ttu-id="320c8-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="320c8-149">The following is a JSON representation of the resource.</span></span>

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
