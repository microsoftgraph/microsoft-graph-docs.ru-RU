---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f5f34664bd721564a8ee63248c65b66123aad98
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507777"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="fd727-103">Тип ресурса Цертификатеаусорити</span><span class="sxs-lookup"><span data-stu-id="fd727-103">certificateAuthority resource type</span></span>

<span data-ttu-id="fd727-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fd727-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd727-105">Представляет центр сертификации.</span><span class="sxs-lookup"><span data-stu-id="fd727-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="fd727-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd727-106">Properties</span></span>

| <span data-ttu-id="fd727-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd727-107">Property</span></span>     | <span data-ttu-id="fd727-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fd727-108">Type</span></span>        | <span data-ttu-id="fd727-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd727-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd727-110">certificate</span><span class="sxs-lookup"><span data-stu-id="fd727-110">certificate</span></span>|<span data-ttu-id="fd727-111">Двоичный</span><span class="sxs-lookup"><span data-stu-id="fd727-111">Binary</span></span>|<span data-ttu-id="fd727-112">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="fd727-112">Required.</span></span> <span data-ttu-id="fd727-113">Строка в кодировке Base64, представляющая общедоступный сертификат.</span><span class="sxs-lookup"><span data-stu-id="fd727-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="fd727-114">цертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="fd727-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="fd727-115">String</span><span class="sxs-lookup"><span data-stu-id="fd727-115">String</span></span>|<span data-ttu-id="fd727-116">URL-адрес списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fd727-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="fd727-117">делтацертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="fd727-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="fd727-118">String</span><span class="sxs-lookup"><span data-stu-id="fd727-118">String</span></span>|<span data-ttu-id="fd727-119">URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fd727-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="fd727-120">исрутаусорити</span><span class="sxs-lookup"><span data-stu-id="fd727-120">isRootAuthority</span></span>|<span data-ttu-id="fd727-121">Логический</span><span class="sxs-lookup"><span data-stu-id="fd727-121">Boolean</span></span>|<span data-ttu-id="fd727-122">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="fd727-122">Required.</span></span> <span data-ttu-id="fd727-123">**true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.</span><span class="sxs-lookup"><span data-stu-id="fd727-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="fd727-124">имени</span><span class="sxs-lookup"><span data-stu-id="fd727-124">issuer</span></span>|<span data-ttu-id="fd727-125">String</span><span class="sxs-lookup"><span data-stu-id="fd727-125">String</span></span>|<span data-ttu-id="fd727-126">Поставщик сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="fd727-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="fd727-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd727-127">Read-only.</span></span> |
|<span data-ttu-id="fd727-128">иссуерски</span><span class="sxs-lookup"><span data-stu-id="fd727-128">issuerSki</span></span>|<span data-ttu-id="fd727-129">String</span><span class="sxs-lookup"><span data-stu-id="fd727-129">String</span></span>|<span data-ttu-id="fd727-130">Идентификатор ключа субъекта сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="fd727-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="fd727-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd727-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd727-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd727-132">JSON representation</span></span>

<span data-ttu-id="fd727-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd727-133">The following is a JSON representation of the resource.</span></span>

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