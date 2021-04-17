---
title: тип ресурса pkcs12CertificateInformation
description: Представляет общедоступные сведения клиентского сертификата Pkcs12.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c649021d8fe66530edb794a859eecd8ed08def3
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883109"
---
# <a name="pkcs12certificateinformation-resource-type"></a><span data-ttu-id="ab5e5-103">тип ресурса pkcs12CertificateInformation</span><span class="sxs-lookup"><span data-stu-id="ab5e5-103">pkcs12CertificateInformation resource type</span></span>

<span data-ttu-id="ab5e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab5e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab5e5-105">Представляет общедоступные сведения сертификата Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-105">Represents the public information of a Pkcs12 certificate.</span></span>

## <a name="properties"></a><span data-ttu-id="ab5e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab5e5-106">Properties</span></span>

|<span data-ttu-id="ab5e5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab5e5-107">Property</span></span>|<span data-ttu-id="ab5e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ab5e5-108">Type</span></span>|<span data-ttu-id="ab5e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab5e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5e5-110">isActive</span><span class="sxs-lookup"><span data-stu-id="ab5e5-110">isActive</span></span>|<span data-ttu-id="ab5e5-111">Логическое</span><span class="sxs-lookup"><span data-stu-id="ab5e5-111">Boolean</span></span>|  <span data-ttu-id="ab5e5-112">Представляет, является ли сертификат активным сертификатом, используемым для вызова соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-112">Represents whether the certificate is the active certificate to be used for calling the API connector.</span></span> <span data-ttu-id="ab5e5-113">Активный сертификат — это самый недавно загруженный сертификат, срок действия которого еще не истек, но срок которого не истек.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-113">The active certificate is the most recently uploaded certificate which is not yet expired but whose notBefore time is in the past.</span></span>|
|<span data-ttu-id="ab5e5-114">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="ab5e5-114">thumbprint</span></span>|<span data-ttu-id="ab5e5-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ab5e5-115">String</span></span>| <span data-ttu-id="ab5e5-116">Отпечаток сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-116">The certificate thumbprint.</span></span> |
|<span data-ttu-id="ab5e5-117">notAfter</span><span class="sxs-lookup"><span data-stu-id="ab5e5-117">notAfter</span></span>|<span data-ttu-id="ab5e5-118">Целое число</span><span class="sxs-lookup"><span data-stu-id="ab5e5-118">Integer</span></span>| <span data-ttu-id="ab5e5-119">Срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-119">The certificate's expiry.</span></span> <span data-ttu-id="ab5e5-120">Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="ab5e5-120">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|
|<span data-ttu-id="ab5e5-121">notBefore</span><span class="sxs-lookup"><span data-stu-id="ab5e5-121">notBefore</span></span>|<span data-ttu-id="ab5e5-122">Целое число</span><span class="sxs-lookup"><span data-stu-id="ab5e5-122">Integer</span></span>| <span data-ttu-id="ab5e5-123">Время выдачи сертификата (не ранее).</span><span class="sxs-lookup"><span data-stu-id="ab5e5-123">The certificate's issue time (not before).</span></span> <span data-ttu-id="ab5e5-124">Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="ab5e5-124">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab5e5-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab5e5-125">JSON representation</span></span>

<span data-ttu-id="ab5e5-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab5e5-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12CertificateInformation"
}
-->

``` json
{
    "isActive": "Boolean",
    "thumbprint": "String",
    "notAfter": "DateTime",
    "notBefore": "DateTime"
}
```
