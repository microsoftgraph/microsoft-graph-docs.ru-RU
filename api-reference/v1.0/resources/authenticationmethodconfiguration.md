---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26d0cd948a69968a7d45b3406b3da7109ffc3f18
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469131"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="2e48c-103">тип ресурса authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e48c-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="2e48c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e48c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e48c-105">Представляет политику метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="2e48c-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="2e48c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e48c-106">Properties</span></span>
|<span data-ttu-id="2e48c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e48c-107">Property</span></span>|<span data-ttu-id="2e48c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2e48c-108">Type</span></span>|<span data-ttu-id="2e48c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e48c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e48c-110">id</span><span class="sxs-lookup"><span data-stu-id="2e48c-110">id</span></span>|<span data-ttu-id="2e48c-111">String</span><span class="sxs-lookup"><span data-stu-id="2e48c-111">String</span></span>|<span data-ttu-id="2e48c-112">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="2e48c-112">The policy name.</span></span>|
|<span data-ttu-id="2e48c-113">state</span><span class="sxs-lookup"><span data-stu-id="2e48c-113">state</span></span>|<span data-ttu-id="2e48c-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="2e48c-114">authenticationMethodState</span></span>|<span data-ttu-id="2e48c-115">Состояние политики.</span><span class="sxs-lookup"><span data-stu-id="2e48c-115">The state of the policy.</span></span> <span data-ttu-id="2e48c-116">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2e48c-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e48c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="2e48c-117">Relationships</span></span>
<span data-ttu-id="2e48c-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2e48c-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e48c-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e48c-119">JSON representation</span></span>
<span data-ttu-id="2e48c-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e48c-120">The following is a JSON representation of the resource.</span></span>
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
