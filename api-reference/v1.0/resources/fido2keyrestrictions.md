---
title: тип ресурса fido2KeyRestrictions
description: Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей безопасности FIDO2.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1781e39952bb3bf7cfb307d06ca3167ff58a2a6
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469453"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="ab92b-103">тип ресурса fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="ab92b-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="ab92b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab92b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab92b-105">Представляет основные ограничения, которые применяются в рамках политики методов проверки подлинности ключей [безопасности FIDO2.](../resources/fido2authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab92b-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ab92b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab92b-106">Properties</span></span>
|<span data-ttu-id="ab92b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab92b-107">Property</span></span>|<span data-ttu-id="ab92b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ab92b-108">Type</span></span>|<span data-ttu-id="ab92b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ab92b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab92b-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="ab92b-110">aaGuids</span></span>|<span data-ttu-id="ab92b-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab92b-111">String collection</span></span>|<span data-ttu-id="ab92b-112">Коллекция GUID-интерфейсов проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ab92b-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="ab92b-113">AADGUID определяет ключевые типы и производителей.</span><span class="sxs-lookup"><span data-stu-id="ab92b-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="ab92b-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="ab92b-114">enforcementType</span></span>|<span data-ttu-id="ab92b-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="ab92b-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="ab92b-116">Тип правоприменения.</span><span class="sxs-lookup"><span data-stu-id="ab92b-116">Enforcement type.</span></span> <span data-ttu-id="ab92b-117">Возможные значения: `allow`, `block`.</span><span class="sxs-lookup"><span data-stu-id="ab92b-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="ab92b-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="ab92b-118">isEnforced</span></span>|<span data-ttu-id="ab92b-119">Логический</span><span class="sxs-lookup"><span data-stu-id="ab92b-119">Boolean</span></span>|<span data-ttu-id="ab92b-120">Определяет, включено ли правоприменительных ключевых элементов.</span><span class="sxs-lookup"><span data-stu-id="ab92b-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab92b-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ab92b-121">Relationships</span></span>
<span data-ttu-id="ab92b-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ab92b-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab92b-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ab92b-123">JSON representation</span></span>
<span data-ttu-id="ab92b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab92b-124">The following is a JSON representation of the resource.</span></span>
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
