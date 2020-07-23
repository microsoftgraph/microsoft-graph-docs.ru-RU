---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6271ae47f94abb0c449dc6bd7a0930468d08d2b5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384726"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="2daaf-103">Тип ресурса Клаудаппсекуритисессионконтрол</span><span class="sxs-lookup"><span data-stu-id="2daaf-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="2daaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2daaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2daaf-105">Управление сеансами, используемое для применения проверок безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="2daaf-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="2daaf-106">Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="2daaf-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2daaf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2daaf-107">Properties</span></span>

| <span data-ttu-id="2daaf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2daaf-108">Property</span></span>     | <span data-ttu-id="2daaf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2daaf-109">Type</span></span>        | <span data-ttu-id="2daaf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2daaf-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2daaf-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2daaf-111">isEnabled</span></span>     |<span data-ttu-id="2daaf-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2daaf-112">Boolean</span></span>      | <span data-ttu-id="2daaf-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="2daaf-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="2daaf-114">клаудаппсекурититипе</span><span class="sxs-lookup"><span data-stu-id="2daaf-114">cloudAppSecurityType</span></span>|<span data-ttu-id="2daaf-115">String</span><span class="sxs-lookup"><span data-stu-id="2daaf-115">String</span></span>| <span data-ttu-id="2daaf-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2daaf-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="2daaf-117">Для получения дополнительных сведений обратитесь [к разделу развертывание приложения условного доступа для популярных приложений](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad).</span><span class="sxs-lookup"><span data-stu-id="2daaf-117">For more information, see [Deploy Conditional Access App Control for featured apps](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2daaf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2daaf-118">Relationships</span></span>

<span data-ttu-id="2daaf-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2daaf-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2daaf-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2daaf-120">JSON representation</span></span>

<span data-ttu-id="2daaf-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2daaf-121">The following is a JSON representation of the resource.</span></span>

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
