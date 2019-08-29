---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf88364ffd8f06783ef98ac32276d948fc6b1791
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667677"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="313e2-103">Тип ресурса Цертификатеаусорити</span><span class="sxs-lookup"><span data-stu-id="313e2-103">certificateAuthority resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="313e2-104">Представляет центр сертификации.</span><span class="sxs-lookup"><span data-stu-id="313e2-104">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="313e2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="313e2-105">Properties</span></span>

| <span data-ttu-id="313e2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="313e2-106">Property</span></span>     | <span data-ttu-id="313e2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="313e2-107">Type</span></span>        | <span data-ttu-id="313e2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="313e2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="313e2-109">certificate</span><span class="sxs-lookup"><span data-stu-id="313e2-109">certificate</span></span>|<span data-ttu-id="313e2-110">Двоичный</span><span class="sxs-lookup"><span data-stu-id="313e2-110">Binary</span></span>|<span data-ttu-id="313e2-111">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="313e2-111">Required.</span></span> <span data-ttu-id="313e2-112">Строка в кодировке Base64, представляющая общедоступный сертификат.</span><span class="sxs-lookup"><span data-stu-id="313e2-112">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="313e2-113">цертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="313e2-113">certificateRevocationListUrl</span></span>|<span data-ttu-id="313e2-114">String.</span><span class="sxs-lookup"><span data-stu-id="313e2-114">String</span></span>|<span data-ttu-id="313e2-115">URL-адрес списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="313e2-115">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="313e2-116">делтацертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="313e2-116">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="313e2-117">String.</span><span class="sxs-lookup"><span data-stu-id="313e2-117">String</span></span>|<span data-ttu-id="313e2-118">URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.</span><span class="sxs-lookup"><span data-stu-id="313e2-118">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="313e2-119">исрутаусорити</span><span class="sxs-lookup"><span data-stu-id="313e2-119">isRootAuthority</span></span>|<span data-ttu-id="313e2-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="313e2-120">Boolean</span></span>|<span data-ttu-id="313e2-121">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="313e2-121">Required.</span></span> <span data-ttu-id="313e2-122">**true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.</span><span class="sxs-lookup"><span data-stu-id="313e2-122">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="313e2-123">имени</span><span class="sxs-lookup"><span data-stu-id="313e2-123">issuer</span></span>|<span data-ttu-id="313e2-124">String.</span><span class="sxs-lookup"><span data-stu-id="313e2-124">String</span></span>|<span data-ttu-id="313e2-125">Поставщик сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="313e2-125">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="313e2-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="313e2-126">Read-only.</span></span> |
|<span data-ttu-id="313e2-127">иссуерски</span><span class="sxs-lookup"><span data-stu-id="313e2-127">issuerSki</span></span>|<span data-ttu-id="313e2-128">String.</span><span class="sxs-lookup"><span data-stu-id="313e2-128">String</span></span>|<span data-ttu-id="313e2-129">Идентификатор ключа субъекта сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="313e2-129">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="313e2-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="313e2-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="313e2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="313e2-131">JSON representation</span></span>

<span data-ttu-id="313e2-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="313e2-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->