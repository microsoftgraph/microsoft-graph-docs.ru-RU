---
title: тип ресурса apiAuthenticationConfigurationBase
description: Представляет базовый тип конфигурации проверки подлинности, используемой для вызова API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 915e1c0c26cee173991d75bc46a1a0230844d2ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507968"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a><span data-ttu-id="4e59e-103">тип ресурса apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="4e59e-103">apiAuthenticationConfigurationBase resource type</span></span>

<span data-ttu-id="4e59e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e59e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e59e-105">Базовый тип для удержания сведений о проверке подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="4e59e-105">The base type to hold authentication information for calling an API.</span></span>

<span data-ttu-id="4e59e-106">Производные типы включают в себя:</span><span class="sxs-lookup"><span data-stu-id="4e59e-106">Derived types include:</span></span>
- <span data-ttu-id="4e59e-107">[basicAuthentication](basicauthentication.md) для базовой проверки подлинности HTTP</span><span class="sxs-lookup"><span data-stu-id="4e59e-107">[basicAuthentication](basicauthentication.md) for HTTP basic authentication</span></span>
- <span data-ttu-id="4e59e-108">[pkcs12certificate](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для создания или отправки соединителя API)</span><span class="sxs-lookup"><span data-stu-id="4e59e-108">[pkcs12certificate](pkcs12certificate.md) for client certificate authentication (used for API connector create or upload)</span></span>
- <span data-ttu-id="4e59e-109">[clientCertificateAuthentication](pkcs12certificate.md) для проверки подлинности сертификатов клиента (используется для получения клиентских сертификатов соединителя API)</span><span class="sxs-lookup"><span data-stu-id="4e59e-109">[clientCertificateAuthentication](pkcs12certificate.md) for client certificate authentication (used for fetching the client certificates of an API connector)</span></span>

## <a name="properties"></a><span data-ttu-id="4e59e-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e59e-110">Properties</span></span>

|<span data-ttu-id="4e59e-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e59e-111">Property</span></span>|<span data-ttu-id="4e59e-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4e59e-112">Type</span></span>|<span data-ttu-id="4e59e-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4e59e-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="4e59e-114">Связи</span><span class="sxs-lookup"><span data-stu-id="4e59e-114">Relationships</span></span>

<span data-ttu-id="4e59e-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e59e-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e59e-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e59e-116">JSON representation</span></span>

<span data-ttu-id="4e59e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e59e-117">The following is a JSON representation of the resource.</span></span>
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
