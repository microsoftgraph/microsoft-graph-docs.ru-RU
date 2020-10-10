---
title: аусентикатионмесодконфигуратионс
description: Объект Аусентикатионмесодконфигуратионс.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 856db11063c3f766f07ff725fe172270449d272d
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418513"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="3a911-103">Тип ресурса Аусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="3a911-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="3a911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a911-105">Представляет политику метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3a911-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3a911-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a911-106">Properties</span></span>
|<span data-ttu-id="3a911-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a911-107">Property</span></span>|<span data-ttu-id="3a911-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3a911-108">Type</span></span>|<span data-ttu-id="3a911-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3a911-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a911-110">id</span><span class="sxs-lookup"><span data-stu-id="3a911-110">id</span></span>|<span data-ttu-id="3a911-111">String</span><span class="sxs-lookup"><span data-stu-id="3a911-111">String</span></span>|<span data-ttu-id="3a911-112">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="3a911-112">The policy name.</span></span>|
|<span data-ttu-id="3a911-113">state</span><span class="sxs-lookup"><span data-stu-id="3a911-113">state</span></span>|<span data-ttu-id="3a911-114">аусентикатионмесодстате</span><span class="sxs-lookup"><span data-stu-id="3a911-114">authenticationMethodState</span></span>|<span data-ttu-id="3a911-115">Состояние политики.</span><span class="sxs-lookup"><span data-stu-id="3a911-115">The state of the policy.</span></span> <span data-ttu-id="3a911-116">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="3a911-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a911-117">Связи</span><span class="sxs-lookup"><span data-stu-id="3a911-117">Relationships</span></span>
<span data-ttu-id="3a911-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3a911-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a911-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3a911-119">JSON representation</span></span>
<span data-ttu-id="3a911-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a911-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
