---
title: тип ресурса clientCertificateAuthentication
description: Представляет конфигурацию для ирисовки клиентаCertificateAuthentication.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69870b1160078495d3b9440260aab1f231041eef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882485"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="70d10-103">тип ресурса clientCertificateAuthentication</span><span class="sxs-lookup"><span data-stu-id="70d10-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="70d10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70d10-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70d10-105">Тип, полученный из apiAuthenticationConfigurationBase, который используется для представления проверки подлинности клиентского сертификата на основе Pkcs12.</span><span class="sxs-lookup"><span data-stu-id="70d10-105">A type derived from apiAuthenticationConfigurationBase that is used to represent a Pkcs12-based client certificate authentication.</span></span> <span data-ttu-id="70d10-106">Это используется для получения общедоступных свойств загруженных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="70d10-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="70d10-107">Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="70d10-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="70d10-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="70d10-108">Properties</span></span>

|<span data-ttu-id="70d10-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="70d10-109">Property</span></span>|<span data-ttu-id="70d10-110">Тип</span><span class="sxs-lookup"><span data-stu-id="70d10-110">Type</span></span>|<span data-ttu-id="70d10-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70d10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70d10-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="70d10-112">certificateList</span></span>| <span data-ttu-id="70d10-113">[коллекция pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md)</span><span class="sxs-lookup"><span data-stu-id="70d10-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="70d10-114">Список сертификатов, загруженных для этого соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="70d10-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70d10-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70d10-115">JSON representation</span></span>

<span data-ttu-id="70d10-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70d10-116">The following is a JSON representation of the resource.</span></span>
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
