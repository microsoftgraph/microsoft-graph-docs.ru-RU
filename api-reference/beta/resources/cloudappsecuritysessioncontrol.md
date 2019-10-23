---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 105a60905bd69317d152d9609e0a95fb78610a35
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638598"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="9d095-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="9d095-103">cloudAppSecuritySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d095-104">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="9d095-104">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="9d095-105">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="9d095-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9d095-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d095-106">Properties</span></span>

| <span data-ttu-id="9d095-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d095-107">Property</span></span>     | <span data-ttu-id="9d095-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d095-108">Type</span></span>        | <span data-ttu-id="9d095-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d095-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d095-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9d095-110">isEnabled</span></span>     |<span data-ttu-id="9d095-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d095-111">Boolean</span></span>      | <span data-ttu-id="9d095-112">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="9d095-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="9d095-113">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="9d095-113">cloudAppSecurityType</span></span>|<span data-ttu-id="9d095-114">String</span><span class="sxs-lookup"><span data-stu-id="9d095-114">String</span></span> | <span data-ttu-id="9d095-115">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="9d095-115">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="9d095-116">Подробнее об этих значениях:https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="9d095-116">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d095-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9d095-117">Relationships</span></span>

<span data-ttu-id="9d095-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9d095-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d095-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9d095-119">JSON representation</span></span>

<span data-ttu-id="9d095-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d095-120">The following is a JSON representation of the resource.</span></span>

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