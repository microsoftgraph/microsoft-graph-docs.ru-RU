---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 691184b1dfbf0323204debd70488d232d77b4f7a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761137"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="74738-103">тип ресурса authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="74738-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="74738-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74738-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74738-105">Представляет политику метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="74738-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="74738-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="74738-106">Properties</span></span>
|<span data-ttu-id="74738-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="74738-107">Property</span></span>|<span data-ttu-id="74738-108">Тип</span><span class="sxs-lookup"><span data-stu-id="74738-108">Type</span></span>|<span data-ttu-id="74738-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74738-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74738-110">id</span><span class="sxs-lookup"><span data-stu-id="74738-110">id</span></span>|<span data-ttu-id="74738-111">String</span><span class="sxs-lookup"><span data-stu-id="74738-111">String</span></span>|<span data-ttu-id="74738-112">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="74738-112">The policy name.</span></span>|
|<span data-ttu-id="74738-113">state</span><span class="sxs-lookup"><span data-stu-id="74738-113">state</span></span>|<span data-ttu-id="74738-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="74738-114">authenticationMethodState</span></span>|<span data-ttu-id="74738-115">Состояние политики.</span><span class="sxs-lookup"><span data-stu-id="74738-115">The state of the policy.</span></span> <span data-ttu-id="74738-116">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="74738-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74738-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="74738-117">Relationships</span></span>
<span data-ttu-id="74738-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74738-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74738-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74738-119">JSON representation</span></span>
<span data-ttu-id="74738-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74738-120">The following is a JSON representation of the resource.</span></span>
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
