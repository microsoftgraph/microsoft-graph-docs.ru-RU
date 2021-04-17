---
title: тип ресурса userFlowApiConnectorConfiguration
description: Представляет соединители API, которые включены для потока пользователей.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b9d9b87bf59a796e8c79875a8506fccdd4d3447b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883311"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="5fe1a-103">тип ресурса userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5fe1a-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="5fe1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fe1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fe1a-105">Определяет API, которые называются в определенных точках пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="5fe1a-105">Defines the APIs that are called at specific points in the user flow.</span></span>  <span data-ttu-id="5fe1a-106">Каждое отношение этого объекта соответствует определенному шагу в потоке пользователей, который можно настроить для вызова соединиттеля API.</span><span class="sxs-lookup"><span data-stu-id="5fe1a-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="5fe1a-107">Связи</span><span class="sxs-lookup"><span data-stu-id="5fe1a-107">Relationships</span></span>

| <span data-ttu-id="5fe1a-108">Связь</span><span class="sxs-lookup"><span data-stu-id="5fe1a-108">Relationship</span></span>            | <span data-ttu-id="5fe1a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5fe1a-109">Type</span></span>                                            | <span data-ttu-id="5fe1a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe1a-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="5fe1a-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="5fe1a-111">postFederationSignup</span></span>    | [<span data-ttu-id="5fe1a-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="5fe1a-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="5fe1a-113">Указывает API для вызова федерации с внешним поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5fe1a-113">Specifies an API to call after federation with an external identity provider.</span></span> <span data-ttu-id="5fe1a-114">Например, API Google, Facebook или Azure AD завершится при регистрации пользователя (не применяется к входу).</span><span class="sxs-lookup"><span data-stu-id="5fe1a-114">For example, a Google, Facebook, or Azure AD API is completed when the user is signing up (does not apply to sign-in).</span></span> |
| <span data-ttu-id="5fe1a-115">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="5fe1a-115">postAttributeCollection</span></span> | [<span data-ttu-id="5fe1a-116">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="5fe1a-116">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="5fe1a-117">Указывает API для вызова после отправки пользователем собранных атрибутов и до создания учетной записи пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="5fe1a-117">Specifies an API to call after a user submits the collected attributes and before the user account is created during sign-up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="5fe1a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fe1a-118">JSON representation</span></span>

<span data-ttu-id="5fe1a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe1a-119">The following is a JSON representation of the resource.</span></span>
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
  ]
}-->
