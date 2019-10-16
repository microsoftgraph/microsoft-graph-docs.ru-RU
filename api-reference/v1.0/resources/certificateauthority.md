---
title: Тип ресурса Цертификатеаусорити
description: Представляет центр сертификации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030e0fbe8fcae0408f51c20882d49e50d825cdb8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539297"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="46c81-103">Тип ресурса Цертификатеаусорити</span><span class="sxs-lookup"><span data-stu-id="46c81-103">certificateAuthority resource type</span></span>

<span data-ttu-id="46c81-104">Представляет центр сертификации.</span><span class="sxs-lookup"><span data-stu-id="46c81-104">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="46c81-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="46c81-105">Properties</span></span>

| <span data-ttu-id="46c81-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="46c81-106">Property</span></span>     | <span data-ttu-id="46c81-107">Тип</span><span class="sxs-lookup"><span data-stu-id="46c81-107">Type</span></span>        | <span data-ttu-id="46c81-108">Описание</span><span class="sxs-lookup"><span data-stu-id="46c81-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46c81-109">certificate</span><span class="sxs-lookup"><span data-stu-id="46c81-109">certificate</span></span>|<span data-ttu-id="46c81-110">Двоичный</span><span class="sxs-lookup"><span data-stu-id="46c81-110">Binary</span></span>|<span data-ttu-id="46c81-111">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="46c81-111">Required.</span></span> <span data-ttu-id="46c81-112">Строка в кодировке Base64, представляющая общедоступный сертификат.</span><span class="sxs-lookup"><span data-stu-id="46c81-112">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="46c81-113">цертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="46c81-113">certificateRevocationListUrl</span></span>|<span data-ttu-id="46c81-114">String</span><span class="sxs-lookup"><span data-stu-id="46c81-114">String</span></span>|<span data-ttu-id="46c81-115">URL-адрес списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="46c81-115">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="46c81-116">делтацертификатеревокатионлистурл</span><span class="sxs-lookup"><span data-stu-id="46c81-116">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="46c81-117">String</span><span class="sxs-lookup"><span data-stu-id="46c81-117">String</span></span>|<span data-ttu-id="46c81-118">URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка ревокатон сертификатов.</span><span class="sxs-lookup"><span data-stu-id="46c81-118">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="46c81-119">исрутаусорити</span><span class="sxs-lookup"><span data-stu-id="46c81-119">isRootAuthority</span></span>|<span data-ttu-id="46c81-120">Логический</span><span class="sxs-lookup"><span data-stu-id="46c81-120">Boolean</span></span>|<span data-ttu-id="46c81-121">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="46c81-121">Required.</span></span> <span data-ttu-id="46c81-122">**true** , если доверенным сертификатом является корневой центр, **false** , если доверенный сертификат является промежуточным.</span><span class="sxs-lookup"><span data-stu-id="46c81-122">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="46c81-123">имени</span><span class="sxs-lookup"><span data-stu-id="46c81-123">issuer</span></span>|<span data-ttu-id="46c81-124">String</span><span class="sxs-lookup"><span data-stu-id="46c81-124">String</span></span>|<span data-ttu-id="46c81-125">Поставщик сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="46c81-125">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="46c81-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46c81-126">Read-only.</span></span> |
|<span data-ttu-id="46c81-127">иссуерски</span><span class="sxs-lookup"><span data-stu-id="46c81-127">issuerSki</span></span>|<span data-ttu-id="46c81-128">String</span><span class="sxs-lookup"><span data-stu-id="46c81-128">String</span></span>|<span data-ttu-id="46c81-129">Идентификатор ключа субъекта сертификата, рассчитанный на основе значения **сертификата** .</span><span class="sxs-lookup"><span data-stu-id="46c81-129">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="46c81-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46c81-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46c81-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46c81-131">JSON representation</span></span>

<span data-ttu-id="46c81-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46c81-132">The following is a JSON representation of the resource.</span></span>

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