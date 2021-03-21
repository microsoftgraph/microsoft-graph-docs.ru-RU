---
title: тип ресурса fido2KeyRestrictions
description: Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fd319b64d124fc2c80c7f851a2e062d3568c2d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964959"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="96bd5-103">тип ресурса fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="96bd5-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="96bd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96bd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96bd5-105">Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей [безопасности FIDO2.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="96bd5-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="96bd5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="96bd5-106">Properties</span></span>
|<span data-ttu-id="96bd5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="96bd5-107">Property</span></span>|<span data-ttu-id="96bd5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="96bd5-108">Type</span></span>|<span data-ttu-id="96bd5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="96bd5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96bd5-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="96bd5-110">aaGuids</span></span>|<span data-ttu-id="96bd5-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96bd5-111">String collection</span></span>|<span data-ttu-id="96bd5-112">Коллекция GUID-интерфейсов проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="96bd5-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="96bd5-113">AADGUID определяет ключевые типы и производителей.</span><span class="sxs-lookup"><span data-stu-id="96bd5-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="96bd5-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="96bd5-114">enforcementType</span></span>|<span data-ttu-id="96bd5-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="96bd5-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="96bd5-116">Тип правоприменения.</span><span class="sxs-lookup"><span data-stu-id="96bd5-116">Enforcement type.</span></span> <span data-ttu-id="96bd5-117">Возможные значения: `allow`, `block`.</span><span class="sxs-lookup"><span data-stu-id="96bd5-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="96bd5-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="96bd5-118">isEnforced</span></span>|<span data-ttu-id="96bd5-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="96bd5-119">Boolean</span></span>|<span data-ttu-id="96bd5-120">Определяет, включено ли правоприменительных ключевых элементов.</span><span class="sxs-lookup"><span data-stu-id="96bd5-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96bd5-121">Связи</span><span class="sxs-lookup"><span data-stu-id="96bd5-121">Relationships</span></span>
<span data-ttu-id="96bd5-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="96bd5-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96bd5-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="96bd5-123">JSON representation</span></span>
<span data-ttu-id="96bd5-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96bd5-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
