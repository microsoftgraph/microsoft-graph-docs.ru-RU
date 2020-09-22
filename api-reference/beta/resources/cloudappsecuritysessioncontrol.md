---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4665fc3456dbd6375ea0ef9651455427e74b732f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034072"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="c7ef5-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="c7ef5-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="c7ef5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7ef5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ef5-105">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="c7ef5-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="c7ef5-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="c7ef5-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c7ef5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7ef5-107">Properties</span></span>

| <span data-ttu-id="c7ef5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ef5-108">Property</span></span>     | <span data-ttu-id="c7ef5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ef5-109">Type</span></span>        | <span data-ttu-id="c7ef5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ef5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c7ef5-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c7ef5-111">isEnabled</span></span>     |<span data-ttu-id="c7ef5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7ef5-112">Boolean</span></span>      | <span data-ttu-id="c7ef5-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="c7ef5-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="c7ef5-114">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="c7ef5-114">cloudAppSecurityType</span></span>|<span data-ttu-id="c7ef5-115">String</span><span class="sxs-lookup"><span data-stu-id="c7ef5-115">String</span></span> | <span data-ttu-id="c7ef5-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="c7ef5-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="c7ef5-117">Подробнее об этих значениях: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="c7ef5-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7ef5-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="c7ef5-118">Relationships</span></span>

<span data-ttu-id="c7ef5-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c7ef5-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7ef5-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7ef5-120">JSON representation</span></span>

<span data-ttu-id="c7ef5-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7ef5-121">The following is a JSON representation of the resource.</span></span>

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

