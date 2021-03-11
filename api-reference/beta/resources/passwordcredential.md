---
title: тип ресурса passwordCredential
description: Содержит учетные данные паролей, связанные с приложением или директором службы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fbc5af586392191e2ab583ad6e723b3ee0789463
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720561"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="b1c80-103">тип ресурса passwordCredential</span><span class="sxs-lookup"><span data-stu-id="b1c80-103">passwordCredential resource type</span></span>

<span data-ttu-id="b1c80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1c80-105">Представляет учетные данные паролей, связанные с приложением или директором службы.</span><span class="sxs-lookup"><span data-stu-id="b1c80-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="b1c80-106">Свойство **passwordCredentials** сущностями application [и](application.md) [servicePrincipal](serviceprincipal.md) — это коллекция **объектов passwordCredential.**</span><span class="sxs-lookup"><span data-stu-id="b1c80-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1c80-107">Использование POST или PATCH для **набора passwordCredential** не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c80-107">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="b1c80-108">Используйте методы addPassword и removePassword, чтобы обновить пароль для приложения или службыPrincipal:</span><span class="sxs-lookup"><span data-stu-id="b1c80-108">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="b1c80-109">приложение: addPassword</span><span class="sxs-lookup"><span data-stu-id="b1c80-109">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="b1c80-110">приложение: removePassword</span><span class="sxs-lookup"><span data-stu-id="b1c80-110">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="b1c80-111">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="b1c80-111">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="b1c80-112">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="b1c80-112">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a><span data-ttu-id="b1c80-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1c80-113">Properties</span></span>
| <span data-ttu-id="b1c80-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1c80-114">Property</span></span>     | <span data-ttu-id="b1c80-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c80-115">Type</span></span>   |<span data-ttu-id="b1c80-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c80-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1c80-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1c80-117">customKeyIdentifier</span></span> | <span data-ttu-id="b1c80-118">Binary</span><span class="sxs-lookup"><span data-stu-id="b1c80-118">Binary</span></span> | <span data-ttu-id="b1c80-119">Не следует использовать.</span><span class="sxs-lookup"><span data-stu-id="b1c80-119">Do not use.</span></span> |
| <span data-ttu-id="b1c80-120">displayName</span><span class="sxs-lookup"><span data-stu-id="b1c80-120">displayName</span></span> | <span data-ttu-id="b1c80-121">String</span><span class="sxs-lookup"><span data-stu-id="b1c80-121">String</span></span> | <span data-ttu-id="b1c80-122">Удобное имя пароля.</span><span class="sxs-lookup"><span data-stu-id="b1c80-122">Friendly name for the password.</span></span> <span data-ttu-id="b1c80-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="b1c80-123">Optional.</span></span> |
| <span data-ttu-id="b1c80-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b1c80-124">endDateTime</span></span> | <span data-ttu-id="b1c80-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1c80-125">DateTimeOffset</span></span> | <span data-ttu-id="b1c80-126">Дата и время, в течение которых истекает срок действия пароля, представлены в формате ISO 8601 и всегда во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="b1c80-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1c80-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b1c80-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b1c80-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="b1c80-128">Optional.</span></span> |
| <span data-ttu-id="b1c80-129">подсказка</span><span class="sxs-lookup"><span data-stu-id="b1c80-129">hint</span></span> | <span data-ttu-id="b1c80-130">String</span><span class="sxs-lookup"><span data-stu-id="b1c80-130">String</span></span> | <span data-ttu-id="b1c80-131">Содержит первые три символа пароля.</span><span class="sxs-lookup"><span data-stu-id="b1c80-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="b1c80-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1c80-132">Read-only.</span></span> |
| <span data-ttu-id="b1c80-133">keyId</span><span class="sxs-lookup"><span data-stu-id="b1c80-133">keyId</span></span> | <span data-ttu-id="b1c80-134">Guid</span><span class="sxs-lookup"><span data-stu-id="b1c80-134">Guid</span></span> | <span data-ttu-id="b1c80-135">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="b1c80-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="b1c80-136">secretText</span><span class="sxs-lookup"><span data-stu-id="b1c80-136">secretText</span></span> | <span data-ttu-id="b1c80-137">String</span><span class="sxs-lookup"><span data-stu-id="b1c80-137">String</span></span> | <span data-ttu-id="b1c80-138">Только для чтения; Содержит надежные пароли, созданные Azure AD длиной 16-64 символов.</span><span class="sxs-lookup"><span data-stu-id="b1c80-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="b1c80-139">Сгенерированное значение пароля возвращается только во время первоначального запроса POST для [добавленияPassword.](../api/application-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="b1c80-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="b1c80-140">В будущем этот пароль не будет извлечен.</span><span class="sxs-lookup"><span data-stu-id="b1c80-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="b1c80-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b1c80-141">startDateTime</span></span> | <span data-ttu-id="b1c80-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1c80-142">DateTimeOffset</span></span> | <span data-ttu-id="b1c80-143">Дата и время, в течение которых пароль становится допустимым.</span><span class="sxs-lookup"><span data-stu-id="b1c80-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="b1c80-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b1c80-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1c80-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b1c80-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b1c80-146">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="b1c80-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="b1c80-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1c80-147">JSON representation</span></span>

<span data-ttu-id="b1c80-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1c80-148">The following is a JSON representation of the resource.</span></span>

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


