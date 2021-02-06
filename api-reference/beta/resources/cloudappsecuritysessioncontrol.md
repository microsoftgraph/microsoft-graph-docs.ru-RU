---
title: Тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для принудительной проверки безопасности облачных приложений.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ba0b0b2d7c2269358bf6d6cd48d6bf6694fc10ab
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128850"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="56c2b-103">Тип ресурса cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="56c2b-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="56c2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56c2b-105">Управление сеансами, используемая для принудительной проверки безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="56c2b-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="56c2b-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="56c2b-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="56c2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="56c2b-107">Properties</span></span>

| <span data-ttu-id="56c2b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="56c2b-108">Property</span></span>     | <span data-ttu-id="56c2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="56c2b-109">Type</span></span>        | <span data-ttu-id="56c2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56c2b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56c2b-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="56c2b-111">isEnabled</span></span>     |<span data-ttu-id="56c2b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="56c2b-112">Boolean</span></span>      | <span data-ttu-id="56c2b-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="56c2b-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="56c2b-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="56c2b-114">cloudAppSecurityType</span></span>|<span data-ttu-id="56c2b-115">Строка</span><span class="sxs-lookup"><span data-stu-id="56c2b-115">String</span></span> | <span data-ttu-id="56c2b-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="56c2b-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="56c2b-117">Узнайте больше об этих значениях здесь: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="56c2b-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="56c2b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="56c2b-118">Relationships</span></span>

<span data-ttu-id="56c2b-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="56c2b-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56c2b-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="56c2b-120">JSON representation</span></span>

<span data-ttu-id="56c2b-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56c2b-121">The following is a JSON representation of the resource.</span></span>

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

