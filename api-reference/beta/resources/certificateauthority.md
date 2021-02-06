---
title: Тип ресурса certificateAuthority
description: Представляет сертификатный орган.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64461015136129de452227cb0a8de5c7180cfb32
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135102"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="d4fe6-103">Тип ресурса certificateAuthority</span><span class="sxs-lookup"><span data-stu-id="d4fe6-103">certificateAuthority resource type</span></span>

<span data-ttu-id="d4fe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4fe6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4fe6-105">Представляет сертификатный орган.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="d4fe6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4fe6-106">Properties</span></span>

| <span data-ttu-id="d4fe6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4fe6-107">Property</span></span>     | <span data-ttu-id="d4fe6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d4fe6-108">Type</span></span>        | <span data-ttu-id="d4fe6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4fe6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4fe6-110">certificate</span><span class="sxs-lookup"><span data-stu-id="d4fe6-110">certificate</span></span>|<span data-ttu-id="d4fe6-111">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d4fe6-111">Binary</span></span>|<span data-ttu-id="d4fe6-112">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-112">Required.</span></span> <span data-ttu-id="d4fe6-113">Строка в коде base64, представляющая общедоступный сертификат.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="d4fe6-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="d4fe6-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="d4fe6-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d4fe6-115">String</span></span>|<span data-ttu-id="d4fe6-116">URL-адрес списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="d4fe6-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="d4fe6-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="d4fe6-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d4fe6-118">String</span></span>|<span data-ttu-id="d4fe6-119">URL-адрес содержит список всех отозванных сертификатов с момента последнего создания полного списка отзыва сертификатов.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="d4fe6-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="d4fe6-120">isRootAuthority</span></span>|<span data-ttu-id="d4fe6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4fe6-121">Boolean</span></span>|<span data-ttu-id="d4fe6-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-122">Required.</span></span> <span data-ttu-id="d4fe6-123">**имеет** true, если доверенный  сертификат является корневым, false, если доверенный сертификат является промежуточным.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="d4fe6-124">issuer</span><span class="sxs-lookup"><span data-stu-id="d4fe6-124">issuer</span></span>|<span data-ttu-id="d4fe6-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d4fe6-125">String</span></span>|<span data-ttu-id="d4fe6-126">Вычисляется из значения **сертификата.**</span><span class="sxs-lookup"><span data-stu-id="d4fe6-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="d4fe6-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-127">Read-only.</span></span> |
|<span data-ttu-id="d4fe6-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="d4fe6-128">issuerSki</span></span>|<span data-ttu-id="d4fe6-129">Строка</span><span class="sxs-lookup"><span data-stu-id="d4fe6-129">String</span></span>|<span data-ttu-id="d4fe6-130">Идентификатор ключа субъекта сертификата, вычисляемого на **ключевых значениях сертификата.**</span><span class="sxs-lookup"><span data-stu-id="d4fe6-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="d4fe6-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4fe6-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4fe6-132">JSON representation</span></span>

<span data-ttu-id="d4fe6-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4fe6-133">The following is a JSON representation of the resource.</span></span>

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

