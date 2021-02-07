---
title: Тип ресурса cloudAppSecuritySessionControl
description: Контроль сеансов, используемый для принудительной проверки безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b1eee93b3f80b6d7d916f38d783ca94cef8e81a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133058"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a><span data-ttu-id="1c35c-103">Тип ресурса cloudAppSecuritySessionControl</span><span class="sxs-lookup"><span data-stu-id="1c35c-103">cloudAppSecuritySessionControl resource type</span></span>

<span data-ttu-id="1c35c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c35c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c35c-105">Управление сеансами, используемая для принудительной проверки безопасности облачных приложений.</span><span class="sxs-lookup"><span data-stu-id="1c35c-105">Session control used to enforce cloud app security checks.</span></span> <span data-ttu-id="1c35c-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="1c35c-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1c35c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c35c-107">Properties</span></span>

| <span data-ttu-id="1c35c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c35c-108">Property</span></span>     | <span data-ttu-id="1c35c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1c35c-109">Type</span></span>        | <span data-ttu-id="1c35c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1c35c-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c35c-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1c35c-111">isEnabled</span></span>     |<span data-ttu-id="1c35c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c35c-112">Boolean</span></span>      | <span data-ttu-id="1c35c-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="1c35c-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="1c35c-114">cloudAppSecurityType</span><span class="sxs-lookup"><span data-stu-id="1c35c-114">cloudAppSecurityType</span></span>|<span data-ttu-id="1c35c-115">String</span><span class="sxs-lookup"><span data-stu-id="1c35c-115">String</span></span>| <span data-ttu-id="1c35c-116">Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1c35c-116">Possible values are: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`.</span></span> <span data-ttu-id="1c35c-117">Дополнительные сведения [см. в теме "Развертывание функции управления приложениями условного доступа для рекомендуемых приложений".](/cloud-app-security/proxy-deployment-aad)</span><span class="sxs-lookup"><span data-stu-id="1c35c-117">For more information, see [Deploy Conditional Access App Control for featured apps](/cloud-app-security/proxy-deployment-aad).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1c35c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1c35c-118">Relationships</span></span>

<span data-ttu-id="1c35c-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1c35c-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c35c-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1c35c-120">JSON representation</span></span>

<span data-ttu-id="1c35c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c35c-121">The following is a JSON representation of the resource.</span></span>

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
