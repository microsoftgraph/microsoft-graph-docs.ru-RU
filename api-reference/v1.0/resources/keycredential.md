---
title: Тип ресурса keyCredential
description: Содержит учетные данные ключа, связанные с приложением или основным компонентом-службой. Свойство **keyCredentials** объектов application и servicePrincipal — это коллекция **объектов keyCredential.**
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 80583c40b61324b2b150c0ab377e4756f227ce39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135900"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="af514-104">Тип ресурса keyCredential</span><span class="sxs-lookup"><span data-stu-id="af514-104">keyCredential resource type</span></span>

<span data-ttu-id="af514-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af514-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af514-106">Содержит учетные данные ключа, связанные с приложением</span><span class="sxs-lookup"><span data-stu-id="af514-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="af514-107">.</span><span class="sxs-lookup"><span data-stu-id="af514-107">.</span></span> <span data-ttu-id="af514-108">Свойство **keyCredentials** [приложения](application.md)</span><span class="sxs-lookup"><span data-stu-id="af514-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="af514-109">объект — это коллекция **keyCredential.**</span><span class="sxs-lookup"><span data-stu-id="af514-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="af514-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="af514-110">Properties</span></span>
| <span data-ttu-id="af514-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="af514-111">Property</span></span>     | <span data-ttu-id="af514-112">Тип</span><span class="sxs-lookup"><span data-stu-id="af514-112">Type</span></span>   |<span data-ttu-id="af514-113">Описание</span><span class="sxs-lookup"><span data-stu-id="af514-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af514-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="af514-114">customKeyIdentifier</span></span>|<span data-ttu-id="af514-115">Binary</span><span class="sxs-lookup"><span data-stu-id="af514-115">Binary</span></span>| <span data-ttu-id="af514-116">Идентификатор пользовательского ключа</span><span class="sxs-lookup"><span data-stu-id="af514-116">Custom key identifier</span></span> |
| <span data-ttu-id="af514-117">displayName</span><span class="sxs-lookup"><span data-stu-id="af514-117">displayName</span></span> | <span data-ttu-id="af514-118">String</span><span class="sxs-lookup"><span data-stu-id="af514-118">String</span></span> | <span data-ttu-id="af514-119">Имя ключа.</span><span class="sxs-lookup"><span data-stu-id="af514-119">Friendly name for the key.</span></span> <span data-ttu-id="af514-120">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="af514-120">Optional.</span></span> |
|<span data-ttu-id="af514-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="af514-121">endDateTime</span></span>|<span data-ttu-id="af514-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af514-122">DateTimeOffset</span></span>|<span data-ttu-id="af514-123">Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="af514-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="af514-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="af514-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="af514-125">keyId</span><span class="sxs-lookup"><span data-stu-id="af514-125">keyId</span></span>|<span data-ttu-id="af514-126">Guid</span><span class="sxs-lookup"><span data-stu-id="af514-126">Guid</span></span>|<span data-ttu-id="af514-127">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="af514-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="af514-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="af514-128">startDateTime</span></span>|<span data-ttu-id="af514-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af514-129">DateTimeOffset</span></span>|<span data-ttu-id="af514-130">Дата и время, когда учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="af514-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="af514-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="af514-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="af514-132">type</span><span class="sxs-lookup"><span data-stu-id="af514-132">type</span></span>|<span data-ttu-id="af514-133">String</span><span class="sxs-lookup"><span data-stu-id="af514-133">String</span></span>|<span data-ttu-id="af514-134">Тип учетных данных ключа; например, "Symmetric".</span><span class="sxs-lookup"><span data-stu-id="af514-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="af514-135">usage</span><span class="sxs-lookup"><span data-stu-id="af514-135">usage</span></span>|<span data-ttu-id="af514-136">String</span><span class="sxs-lookup"><span data-stu-id="af514-136">String</span></span>|<span data-ttu-id="af514-137">Строка, описывая назначение, для которого можно использовать ключ; например, "Verify".</span><span class="sxs-lookup"><span data-stu-id="af514-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="af514-138">key</span><span class="sxs-lookup"><span data-stu-id="af514-138">key</span></span>|<span data-ttu-id="af514-139">Двоичный</span><span class="sxs-lookup"><span data-stu-id="af514-139">Binary</span></span>| <span data-ttu-id="af514-140">Необработанные данные сертификата в массиве byte, преобразованных в строку Base64; например, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` .</span><span class="sxs-lookup"><span data-stu-id="af514-140">The certificate's raw data in byte array converted to Base64 string; for example, `[System.Convert]::ToBase64String($Cert.GetRawCertData())`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="af514-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af514-141">JSON representation</span></span>

<span data-ttu-id="af514-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af514-142">Here is a JSON representation of the resource</span></span>

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

