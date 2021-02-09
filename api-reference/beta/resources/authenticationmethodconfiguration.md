---
title: authenticationMethodConfigurations
description: Объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cda2cda7756bb795c93e10dddbd344e5a4a92ed2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159141"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="33eff-103">Тип ресурса authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="33eff-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="33eff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33eff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33eff-105">Представляет политику метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="33eff-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="33eff-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="33eff-106">Properties</span></span>
|<span data-ttu-id="33eff-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="33eff-107">Property</span></span>|<span data-ttu-id="33eff-108">Тип</span><span class="sxs-lookup"><span data-stu-id="33eff-108">Type</span></span>|<span data-ttu-id="33eff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="33eff-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33eff-110">id</span><span class="sxs-lookup"><span data-stu-id="33eff-110">id</span></span>|<span data-ttu-id="33eff-111">String</span><span class="sxs-lookup"><span data-stu-id="33eff-111">String</span></span>|<span data-ttu-id="33eff-112">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="33eff-112">The policy name.</span></span>|
|<span data-ttu-id="33eff-113">state</span><span class="sxs-lookup"><span data-stu-id="33eff-113">state</span></span>|<span data-ttu-id="33eff-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="33eff-114">authenticationMethodState</span></span>|<span data-ttu-id="33eff-115">Состояние политики.</span><span class="sxs-lookup"><span data-stu-id="33eff-115">The state of the policy.</span></span> <span data-ttu-id="33eff-116">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="33eff-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33eff-117">Связи</span><span class="sxs-lookup"><span data-stu-id="33eff-117">Relationships</span></span>
<span data-ttu-id="33eff-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33eff-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33eff-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="33eff-119">JSON representation</span></span>
<span data-ttu-id="33eff-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33eff-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
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
