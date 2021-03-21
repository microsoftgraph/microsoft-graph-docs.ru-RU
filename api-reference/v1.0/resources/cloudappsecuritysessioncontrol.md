---
title: тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c52322928b5ef2e2538031ae8c251bc9c1a4caac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962513"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="c1bff-103">тип ресурса cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="c1bff-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="c1bff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1bff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1bff-105">Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="c1bff-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="c1bff-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="c1bff-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c1bff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1bff-107">Properties</span></span>

| <span data-ttu-id="c1bff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1bff-108">Property</span></span>     | <span data-ttu-id="c1bff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1bff-109">Type</span></span>        | <span data-ttu-id="c1bff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1bff-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1bff-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c1bff-111">isEnabled</span></span>     |<span data-ttu-id="c1bff-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1bff-112">Boolean</span></span>      | <span data-ttu-id="c1bff-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="c1bff-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="c1bff-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="c1bff-114">cloudAppSecurityType</span></span>|<span data-ttu-id="c1bff-115">cloudAppSecuritySessionControlType</span><span class="sxs-lookup"><span data-stu-id="c1bff-115">cloudAppSecuritySessionControlType</span></span>| <span data-ttu-id="c1bff-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c1bff-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="c1bff-117">Дополнительные сведения см. в [приложении Deploy Conditional Access App Control для рекомендуемых приложений.](/cloud-app-security/proxy-deployment-aad)</span><span class="sxs-lookup"><span data-stu-id="c1bff-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c1bff-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c1bff-118">Relationships</span></span>

<span data-ttu-id="c1bff-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c1bff-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1bff-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1bff-120">JSON representation</span></span>

<span data-ttu-id="c1bff-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1bff-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
