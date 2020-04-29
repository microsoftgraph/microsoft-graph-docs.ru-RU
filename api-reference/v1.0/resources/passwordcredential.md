---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ec0bc1e6057e1bc9b55b1af90ff0056401f88ff1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397207"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="1653e-103">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="1653e-103">passwordCredential resource type</span></span>

<span data-ttu-id="1653e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1653e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1653e-105">Представляет учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="1653e-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="1653e-106">Свойство **пассвордкредентиалс** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="1653e-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="1653e-107">сущность — это коллекция объектов **пассвордкредентиал** .</span><span class="sxs-lookup"><span data-stu-id="1653e-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1653e-108">Использование POST или PATCH для установки **пассвордкредентиал** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1653e-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="1653e-109">Использование методов Аддпассворд и Ремовепассворд для обновления пароля приложения</span><span class="sxs-lookup"><span data-stu-id="1653e-109">Use the addPassword and removePassword methods to update the password for an application</span></span><!--or a servicePrincipal--><span data-ttu-id="1653e-110">:</span><span class="sxs-lookup"><span data-stu-id="1653e-110">:</span></span>
>
> - [<span data-ttu-id="1653e-111">Приложение: Аддпассворд</span><span class="sxs-lookup"><span data-stu-id="1653e-111">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="1653e-112">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="1653e-112">application: removePassword</span></span>](../api/application-removepassword.md)
<!--
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a><span data-ttu-id="1653e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="1653e-113">Properties</span></span>
| <span data-ttu-id="1653e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="1653e-114">Property</span></span>     | <span data-ttu-id="1653e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="1653e-115">Type</span></span>   |<span data-ttu-id="1653e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1653e-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1653e-117">кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="1653e-117">customKeyIdentifier</span></span> | <span data-ttu-id="1653e-118">Binary</span><span class="sxs-lookup"><span data-stu-id="1653e-118">Binary</span></span> | <span data-ttu-id="1653e-119">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="1653e-119">Do not use.</span></span> |
| <span data-ttu-id="1653e-120">displayName</span><span class="sxs-lookup"><span data-stu-id="1653e-120">displayName</span></span> | <span data-ttu-id="1653e-121">String</span><span class="sxs-lookup"><span data-stu-id="1653e-121">String</span></span> | <span data-ttu-id="1653e-122">Понятное имя для пароля.</span><span class="sxs-lookup"><span data-stu-id="1653e-122">Friendly name for the password.</span></span> <span data-ttu-id="1653e-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="1653e-123">Optional.</span></span> |
| <span data-ttu-id="1653e-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1653e-124">endDateTime</span></span> | <span data-ttu-id="1653e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1653e-125">DateTimeOffset</span></span> | <span data-ttu-id="1653e-126">Дата и время истечения срока действия пароля, представленного в формате ISO 8601, и всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1653e-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1653e-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1653e-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1653e-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="1653e-128">Optional.</span></span> |
| <span data-ttu-id="1653e-129">сказок</span><span class="sxs-lookup"><span data-stu-id="1653e-129">hint</span></span> | <span data-ttu-id="1653e-130">String</span><span class="sxs-lookup"><span data-stu-id="1653e-130">String</span></span> | <span data-ttu-id="1653e-131">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="1653e-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="1653e-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1653e-132">Read-only.</span></span> |
| <span data-ttu-id="1653e-133">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="1653e-133">keyId</span></span> | <span data-ttu-id="1653e-134">GUID</span><span class="sxs-lookup"><span data-stu-id="1653e-134">Guid</span></span> | <span data-ttu-id="1653e-135">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="1653e-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="1653e-136">секреттекст</span><span class="sxs-lookup"><span data-stu-id="1653e-136">secretText</span></span> | <span data-ttu-id="1653e-137">String</span><span class="sxs-lookup"><span data-stu-id="1653e-137">String</span></span> | <span data-ttu-id="1653e-138">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="1653e-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="1653e-139">Созданное значение пароля возвращается только во время начального запроса POST в [аддпассворд](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="1653e-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="1653e-140">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="1653e-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="1653e-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1653e-141">startDateTime</span></span> | <span data-ttu-id="1653e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1653e-142">DateTimeOffset</span></span> | <span data-ttu-id="1653e-143">Дата и время, когда пароль становится действительным.</span><span class="sxs-lookup"><span data-stu-id="1653e-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="1653e-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1653e-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1653e-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1653e-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="1653e-146">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="1653e-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="1653e-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1653e-147">JSON representation</span></span>

<span data-ttu-id="1653e-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1653e-148">The following is a JSON representation of the resource.</span></span>

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
