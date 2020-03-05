---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35f031498fb3a2f4f9c3a48d0102d57081b7c4d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507651"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="e98dc-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="e98dc-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="e98dc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e98dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e98dc-105">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="e98dc-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="e98dc-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="e98dc-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e98dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e98dc-107">Properties</span></span>

| <span data-ttu-id="e98dc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e98dc-108">Property</span></span>     | <span data-ttu-id="e98dc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e98dc-109">Type</span></span>        | <span data-ttu-id="e98dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e98dc-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e98dc-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e98dc-111">isEnabled</span></span>     |<span data-ttu-id="e98dc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e98dc-112">Boolean</span></span>      | <span data-ttu-id="e98dc-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="e98dc-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e98dc-114">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="e98dc-114">cloudAppSecurityType</span></span>|<span data-ttu-id="e98dc-115">String</span><span class="sxs-lookup"><span data-stu-id="e98dc-115">String</span></span> | <span data-ttu-id="e98dc-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="e98dc-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="e98dc-117">Подробнее об этих значениях:https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="e98dc-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="e98dc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e98dc-118">Relationships</span></span>

<span data-ttu-id="e98dc-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e98dc-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e98dc-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e98dc-120">JSON representation</span></span>

<span data-ttu-id="e98dc-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e98dc-121">The following is a JSON representation of the resource.</span></span>

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