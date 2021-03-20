---
title: тип ресурса cloudAppSecuritySessionControl
description: Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 630c558981b3dc9bbb0ec48c9a81ff74868c43bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941836"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="54fb2-103">тип ресурса cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="54fb2-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="54fb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54fb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fb2-105">Управление сеансами, используемая для обеспечения проверки безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="54fb2-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="54fb2-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="54fb2-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54fb2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54fb2-107">Properties</span></span>

| <span data-ttu-id="54fb2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54fb2-108">Property</span></span>     | <span data-ttu-id="54fb2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54fb2-109">Type</span></span>        | <span data-ttu-id="54fb2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54fb2-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54fb2-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="54fb2-111">isEnabled</span></span>     |<span data-ttu-id="54fb2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="54fb2-112">Boolean</span></span>      | <span data-ttu-id="54fb2-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="54fb2-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="54fb2-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="54fb2-114">cloudAppSecurityType</span></span>|<span data-ttu-id="54fb2-115">cloudAppSecuritySessionControlType</span><span class="sxs-lookup"><span data-stu-id="54fb2-115">cloudAppSecuritySessionControlType</span></span>| <span data-ttu-id="54fb2-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span><span class="sxs-lookup"><span data-stu-id="54fb2-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`.</span></span> <span data-ttu-id="54fb2-117">Дополнительные данные об этих значениях можно узнать здесь: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span><span class="sxs-lookup"><span data-stu-id="54fb2-117">Learn more about these values here: https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad#step-1-create-an-azure-ad-conditional-access-test-policy-</span></span> |

## <a name="relationships"></a><span data-ttu-id="54fb2-118">Связи</span><span class="sxs-lookup"><span data-stu-id="54fb2-118">Relationships</span></span>

<span data-ttu-id="54fb2-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54fb2-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54fb2-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="54fb2-120">JSON representation</span></span>

<span data-ttu-id="54fb2-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54fb2-121">The following is a JSON representation of the resource.</span></span>

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

