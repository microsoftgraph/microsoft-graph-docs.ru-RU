---
title: тип ресурса keyCredential
description: Содержит ключевые учетные данные, связанные с приложением или директором службы. Свойство **keyCredentials** сущностями приложения и servicePrincipal — это коллекция **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 05b0aa71059bcf0ef974e49fb012a3815386b9be
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722239"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="8fa72-104">тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="8fa72-104">keyCredential resource type</span></span>

<span data-ttu-id="8fa72-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fa72-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fa72-106">Содержит ключевые учетные данные, связанные с приложением</span><span class="sxs-lookup"><span data-stu-id="8fa72-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="8fa72-107">.</span><span class="sxs-lookup"><span data-stu-id="8fa72-107">.</span></span> <span data-ttu-id="8fa72-108">Свойство **keyCredentials** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="8fa72-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="8fa72-109">объект — это коллекция **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="8fa72-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="8fa72-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fa72-110">Properties</span></span>
| <span data-ttu-id="8fa72-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fa72-111">Property</span></span>     | <span data-ttu-id="8fa72-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8fa72-112">Type</span></span>   |<span data-ttu-id="8fa72-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8fa72-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fa72-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="8fa72-114">customKeyIdentifier</span></span>|<span data-ttu-id="8fa72-115">Binary</span><span class="sxs-lookup"><span data-stu-id="8fa72-115">Binary</span></span>| <span data-ttu-id="8fa72-116">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="8fa72-116">Custom key identifier</span></span> |
| <span data-ttu-id="8fa72-117">displayName</span><span class="sxs-lookup"><span data-stu-id="8fa72-117">displayName</span></span> | <span data-ttu-id="8fa72-118">String</span><span class="sxs-lookup"><span data-stu-id="8fa72-118">String</span></span> | <span data-ttu-id="8fa72-119">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="8fa72-119">Friendly name for the key.</span></span> <span data-ttu-id="8fa72-120">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8fa72-120">Optional.</span></span> |
|<span data-ttu-id="8fa72-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa72-121">endDateTime</span></span>|<span data-ttu-id="8fa72-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fa72-122">DateTimeOffset</span></span>|<span data-ttu-id="8fa72-123">Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="8fa72-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fa72-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8fa72-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8fa72-125">keyId</span><span class="sxs-lookup"><span data-stu-id="8fa72-125">keyId</span></span>|<span data-ttu-id="8fa72-126">Guid</span><span class="sxs-lookup"><span data-stu-id="8fa72-126">Guid</span></span>|<span data-ttu-id="8fa72-127">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="8fa72-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="8fa72-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8fa72-128">startDateTime</span></span>|<span data-ttu-id="8fa72-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fa72-129">DateTimeOffset</span></span>|<span data-ttu-id="8fa72-130">Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="8fa72-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fa72-131">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8fa72-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8fa72-132">type</span><span class="sxs-lookup"><span data-stu-id="8fa72-132">type</span></span>|<span data-ttu-id="8fa72-133">String</span><span class="sxs-lookup"><span data-stu-id="8fa72-133">String</span></span>|<span data-ttu-id="8fa72-134">Тип учетных данных ключей; например, "Симметричный".</span><span class="sxs-lookup"><span data-stu-id="8fa72-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="8fa72-135">использование</span><span class="sxs-lookup"><span data-stu-id="8fa72-135">usage</span></span>|<span data-ttu-id="8fa72-136">String</span><span class="sxs-lookup"><span data-stu-id="8fa72-136">String</span></span>|<span data-ttu-id="8fa72-137">Строка, описываемая цель, для которой можно использовать ключ; например, "Проверка".</span><span class="sxs-lookup"><span data-stu-id="8fa72-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="8fa72-138">key</span><span class="sxs-lookup"><span data-stu-id="8fa72-138">key</span></span>|<span data-ttu-id="8fa72-139">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8fa72-139">Binary</span></span>| <span data-ttu-id="8fa72-140">Необработанные данные сертификата в массиве byte, преобразованных в строку Base64; например, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` .</span><span class="sxs-lookup"><span data-stu-id="8fa72-140">The certificate's raw data in byte array converted to Base64 string; for example, `[System.Convert]::ToBase64String($Cert.GetRawCertData())`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fa72-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fa72-141">JSON representation</span></span>

<span data-ttu-id="8fa72-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fa72-142">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

