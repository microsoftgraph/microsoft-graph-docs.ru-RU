---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 114e788e12ab8f633bc6350b08140f9d5e4fe8a3
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581269"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="e1759-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="e1759-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="e1759-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1759-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1759-105">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="e1759-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="e1759-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="e1759-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1759-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1759-107">Properties</span></span>

| <span data-ttu-id="e1759-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1759-108">Property</span></span>     | <span data-ttu-id="e1759-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e1759-109">Type</span></span>        | <span data-ttu-id="e1759-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e1759-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1759-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e1759-111">isEnabled</span></span>     |<span data-ttu-id="e1759-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1759-112">Boolean</span></span>      | <span data-ttu-id="e1759-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="e1759-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e1759-114">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="e1759-114">cloudAppSecurityType</span></span>|<span data-ttu-id="e1759-115">String</span><span class="sxs-lookup"><span data-stu-id="e1759-115">String</span></span>| <span data-ttu-id="e1759-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e1759-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="e1759-117">Для получения дополнительных сведений обратитесь [к разделу развертывание приложения условного доступа для популярных приложений](/cloud-app-security/proxy-deployment-aad).</span><span class="sxs-lookup"><span data-stu-id="e1759-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e1759-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e1759-118">Relationships</span></span>

<span data-ttu-id="e1759-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e1759-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1759-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e1759-120">JSON representation</span></span>

<span data-ttu-id="e1759-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1759-121">The following is a JSON representation of the resource.</span></span>

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