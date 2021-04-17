---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a9e48d38e7ad69d6790b3b9dddb85960c964ad91
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883319"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a><span data-ttu-id="025a3-103">тип ресурса apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="025a3-103">apiAuthenticationConfigurationBase resource type</span></span>

<span data-ttu-id="025a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="025a3-105">Базовый тип для удержания сведений о проверке подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="025a3-105">The base type to hold authentication information for calling an API.</span></span>

<span data-ttu-id="025a3-106">Производные типы включают в себя:</span><span class="sxs-lookup"><span data-stu-id="025a3-106">Derived types include:</span></span>
- <span data-ttu-id="025a3-107">[basicAuthentication](basicauthentication.md) для базовой проверки подлинности HTTP</span><span class="sxs-lookup"><span data-stu-id="025a3-107">[basicAuthentication](basicauthentication.md) for HTTP basic authentication</span></span>
- <span data-ttu-id="025a3-108">[pkcs12certificate](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для создания или отправки соединителя API)</span><span class="sxs-lookup"><span data-stu-id="025a3-108">[pkcs12certificate](pkcs12certificate.md) for client certificate authentication (used for API connector create or upload)</span></span>
- <span data-ttu-id="025a3-109">[clientCertificateAuthentication](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для получения клиентских сертификатов соединителя API)</span><span class="sxs-lookup"><span data-stu-id="025a3-109">[clientCertificateAuthentication](pkcs12certificate.md) for client certificate authentication (used for fetching the client certificates of an API connector)</span></span>

## <a name="properties"></a><span data-ttu-id="025a3-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="025a3-110">Properties</span></span>

|<span data-ttu-id="025a3-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="025a3-111">Property</span></span>|<span data-ttu-id="025a3-112">Тип</span><span class="sxs-lookup"><span data-stu-id="025a3-112">Type</span></span>|<span data-ttu-id="025a3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="025a3-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="025a3-114">Связи</span><span class="sxs-lookup"><span data-stu-id="025a3-114">Relationships</span></span>

<span data-ttu-id="025a3-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="025a3-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="025a3-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="025a3-116">JSON representation</span></span>

<span data-ttu-id="025a3-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="025a3-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
