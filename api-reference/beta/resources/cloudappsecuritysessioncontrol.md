---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fffabf697a8cb8b06cf89b73ec5afc0043e41ffc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467953"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="5e358-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="5e358-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="5e358-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e358-105">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="5e358-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="5e358-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="5e358-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e358-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e358-107">Properties</span></span>

| <span data-ttu-id="5e358-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e358-108">Property</span></span>     | <span data-ttu-id="5e358-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e358-109">Type</span></span>        | <span data-ttu-id="5e358-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e358-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e358-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5e358-111">isEnabled</span></span>     |<span data-ttu-id="5e358-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e358-112">Boolean</span></span>      | <span data-ttu-id="5e358-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="5e358-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="5e358-114">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="5e358-114">cloudAppSecurityType</span></span>|<span data-ttu-id="5e358-115">String</span><span class="sxs-lookup"><span data-stu-id="5e358-115">String</span></span> | <span data-ttu-id="5e358-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="5e358-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="5e358-117">Подробнее об этих значениях:https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="5e358-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e358-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e358-118">Relationships</span></span>

<span data-ttu-id="5e358-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5e358-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e358-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5e358-120">JSON representation</span></span>

<span data-ttu-id="5e358-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e358-121">The following is a JSON representation of the resource.</span></span>

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