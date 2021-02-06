---
title: Тип ресурса fido2KeyRestrictions
description: Представляет ключевые ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a40a185f688038d3c849113ae8e9b53c4f0652f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133800"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="8d41b-103">Тип ресурса fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="8d41b-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="8d41b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d41b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d41b-105">Представляет ключевые ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности [FIDO2.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d41b-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d41b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d41b-106">Properties</span></span>
|<span data-ttu-id="8d41b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d41b-107">Property</span></span>|<span data-ttu-id="8d41b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8d41b-108">Type</span></span>|<span data-ttu-id="8d41b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8d41b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d41b-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="8d41b-110">aaGuids</span></span>|<span data-ttu-id="8d41b-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8d41b-111">String collection</span></span>|<span data-ttu-id="8d41b-112">Коллекция GUID аутентификации.</span><span class="sxs-lookup"><span data-stu-id="8d41b-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="8d41b-113">AADGUID определяют ключевые типы и изготовителей.</span><span class="sxs-lookup"><span data-stu-id="8d41b-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="8d41b-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="8d41b-114">enforcementType</span></span>|<span data-ttu-id="8d41b-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="8d41b-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="8d41b-116">Тип принуителя.</span><span class="sxs-lookup"><span data-stu-id="8d41b-116">Enforcement type.</span></span> <span data-ttu-id="8d41b-117">Возможные значения: `allow`, `block`.</span><span class="sxs-lookup"><span data-stu-id="8d41b-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="8d41b-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="8d41b-118">isEnforced</span></span>|<span data-ttu-id="8d41b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d41b-119">Boolean</span></span>|<span data-ttu-id="8d41b-120">Определяет, включено ли настроено правопримение ключа.</span><span class="sxs-lookup"><span data-stu-id="8d41b-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d41b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8d41b-121">Relationships</span></span>
<span data-ttu-id="8d41b-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d41b-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d41b-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d41b-123">JSON representation</span></span>
<span data-ttu-id="8d41b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d41b-124">The following is a JSON representation of the resource.</span></span>
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
