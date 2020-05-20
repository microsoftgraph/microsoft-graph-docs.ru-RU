---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: c9611c85f45dcd597ab81c325936a4a8a9075642
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290134"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="358cf-103">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="358cf-103">passwordCredential resource type</span></span>

<span data-ttu-id="358cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="358cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="358cf-105">Представляет учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="358cf-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="358cf-106">Свойство **пассвордкредентиалс** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="358cf-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="358cf-107">сущность — это коллекция объектов **пассвордкредентиал** .</span><span class="sxs-lookup"><span data-stu-id="358cf-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="358cf-108">Использование POST или PATCH для установки **пассвордкредентиал** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="358cf-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="358cf-109">Используйте методы Аддпассворд и Ремовепассворд для обновления пароля приложения или servicePrincipal:</span><span class="sxs-lookup"><span data-stu-id="358cf-109">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="358cf-110">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="358cf-110">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="358cf-111">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="358cf-111">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="358cf-112">servicePrincipal: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="358cf-112">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="358cf-113">servicePrincipal: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="358cf-113">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a><span data-ttu-id="358cf-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="358cf-114">Properties</span></span>
| <span data-ttu-id="358cf-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="358cf-115">Property</span></span>     | <span data-ttu-id="358cf-116">Тип</span><span class="sxs-lookup"><span data-stu-id="358cf-116">Type</span></span>   |<span data-ttu-id="358cf-117">Описание</span><span class="sxs-lookup"><span data-stu-id="358cf-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="358cf-118">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="358cf-118">customKeyIdentifier</span></span> | <span data-ttu-id="358cf-119">Binary</span><span class="sxs-lookup"><span data-stu-id="358cf-119">Binary</span></span> | <span data-ttu-id="358cf-120">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="358cf-120">Do not use.</span></span> |
| <span data-ttu-id="358cf-121">displayName</span><span class="sxs-lookup"><span data-stu-id="358cf-121">displayName</span></span> | <span data-ttu-id="358cf-122">String</span><span class="sxs-lookup"><span data-stu-id="358cf-122">String</span></span> | <span data-ttu-id="358cf-123">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="358cf-123">Friendly name for the password.</span></span> <span data-ttu-id="358cf-124">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="358cf-124">Optional.</span></span> |
| <span data-ttu-id="358cf-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="358cf-125">endDateTime</span></span> | <span data-ttu-id="358cf-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358cf-126">DateTimeOffset</span></span> | <span data-ttu-id="358cf-127">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="358cf-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="358cf-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="358cf-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="358cf-129">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="358cf-129">Optional.</span></span> |
| <span data-ttu-id="358cf-130">сказок</span><span class="sxs-lookup"><span data-stu-id="358cf-130">hint</span></span> | <span data-ttu-id="358cf-131">String</span><span class="sxs-lookup"><span data-stu-id="358cf-131">String</span></span> | <span data-ttu-id="358cf-132">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="358cf-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="358cf-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="358cf-133">Read-only.</span></span> |
| <span data-ttu-id="358cf-134">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="358cf-134">keyId</span></span> | <span data-ttu-id="358cf-135">Guid</span><span class="sxs-lookup"><span data-stu-id="358cf-135">Guid</span></span> | <span data-ttu-id="358cf-136">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="358cf-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="358cf-137">секреттекст</span><span class="sxs-lookup"><span data-stu-id="358cf-137">secretText</span></span> | <span data-ttu-id="358cf-138">String</span><span class="sxs-lookup"><span data-stu-id="358cf-138">String</span></span> | <span data-ttu-id="358cf-139">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="358cf-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="358cf-140">Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="358cf-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="358cf-141">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="358cf-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="358cf-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="358cf-142">startDateTime</span></span> | <span data-ttu-id="358cf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358cf-143">DateTimeOffset</span></span> | <span data-ttu-id="358cf-144">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="358cf-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="358cf-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="358cf-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="358cf-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="358cf-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="358cf-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="358cf-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="358cf-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="358cf-148">JSON representation</span></span>

<span data-ttu-id="358cf-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="358cf-149">The following is a JSON representation of the resource.</span></span>

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
