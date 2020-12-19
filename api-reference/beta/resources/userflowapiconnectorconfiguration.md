---
title: Тип ресурса userFlowApiConnectorConfiguration
description: Представляет, какие соединители API включены для пользовательского потока.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 00b37f1b4bff0edf8aa85d79a01e23169b45dbcf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720461"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="2e416-103">Тип ресурса userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e416-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="2e416-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e416-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e416-105">Определяет, какие API-интерфейсы будут вызваны в определенных точках пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="2e416-105">Defines which APIs are called at specific points in the user flow.</span></span>  <span data-ttu-id="2e416-106">Каждая связь этого объекта соответствует определенному шагу в пользовательском потоке, который можно настроить для вызова соединители API.</span><span class="sxs-lookup"><span data-stu-id="2e416-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="2e416-107">Отношения</span><span class="sxs-lookup"><span data-stu-id="2e416-107">Relationships</span></span>

| <span data-ttu-id="2e416-108">Связь</span><span class="sxs-lookup"><span data-stu-id="2e416-108">Relationship</span></span>            | <span data-ttu-id="2e416-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e416-109">Type</span></span>                                            | <span data-ttu-id="2e416-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e416-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2e416-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="2e416-111">postFederationSignup</span></span>    | [<span data-ttu-id="2e416-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="2e416-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="2e416-113">Указывает API, который будет вызываться после федерации с внешним поставщиком удостоверений (например, Google, Facebook или Azure AD), после регистрации пользователя (не применяется для регистрации).</span><span class="sxs-lookup"><span data-stu-id="2e416-113">Specifies an API to call after federation with an external identity provider (like Google, Facebook, or Azure AD) is completed when user is signing up (does not apply to sign in).</span></span> |
| <span data-ttu-id="2e416-114">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="2e416-114">postAttributeCollection</span></span> | [<span data-ttu-id="2e416-115">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="2e416-115">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="2e416-116">Указывает API, который будет вызываться после отправки пользователем собранных атрибутов и до создания пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="2e416-116">Specifies an API to call after a user submits collected attributes and before the user is created during sign up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="2e416-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e416-117">JSON representation</span></span>

<span data-ttu-id="2e416-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e416-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: Resource userFlowApiConnectorConfiguration has documented navigation properties, but we thought it was a complex type!"
  ]
}-->
