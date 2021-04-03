---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для получения клиентаCertificateAuthentication в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509413"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="20623-103">тип ресурса clientCertificateAuthentication</span><span class="sxs-lookup"><span data-stu-id="20623-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="20623-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20623-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20623-105">Тип, полученный из apiAuthenticationConfigurationBase, который используется для представления проверки подлинности клиентского сертификата на основе Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="20623-105">A type derived from apiAuthenticationConfigurationBase which is used to represent Pkcs12 based client certificate authentication.</span></span> <span data-ttu-id="20623-106">Это используется для получения общедоступных свойств загруженных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="20623-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="20623-107">Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="20623-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20623-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="20623-108">Properties</span></span>

|<span data-ttu-id="20623-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="20623-109">Property</span></span>|<span data-ttu-id="20623-110">Тип</span><span class="sxs-lookup"><span data-stu-id="20623-110">Type</span></span>|<span data-ttu-id="20623-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20623-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20623-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="20623-112">certificateList</span></span>| <span data-ttu-id="20623-113">[коллекция pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)</span><span class="sxs-lookup"><span data-stu-id="20623-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="20623-114">Список сертификатов, загруженных для этого соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="20623-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20623-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20623-115">JSON representation</span></span>

<span data-ttu-id="20623-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20623-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
