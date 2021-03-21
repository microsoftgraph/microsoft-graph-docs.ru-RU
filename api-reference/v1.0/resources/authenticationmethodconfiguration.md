---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 083ace96234a724fc4c9f6e1cdda0cbd8a99e22a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964952"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="89564-103">тип ресурса authenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="89564-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="89564-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89564-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89564-105">Представляет политику метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="89564-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="89564-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="89564-106">Properties</span></span>
|<span data-ttu-id="89564-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="89564-107">Property</span></span>|<span data-ttu-id="89564-108">Тип</span><span class="sxs-lookup"><span data-stu-id="89564-108">Type</span></span>|<span data-ttu-id="89564-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89564-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89564-110">id</span><span class="sxs-lookup"><span data-stu-id="89564-110">id</span></span>|<span data-ttu-id="89564-111">String</span><span class="sxs-lookup"><span data-stu-id="89564-111">String</span></span>|<span data-ttu-id="89564-112">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="89564-112">The policy name.</span></span>|
|<span data-ttu-id="89564-113">state</span><span class="sxs-lookup"><span data-stu-id="89564-113">state</span></span>|<span data-ttu-id="89564-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="89564-114">authenticationMethodState</span></span>|<span data-ttu-id="89564-115">Состояние политики.</span><span class="sxs-lookup"><span data-stu-id="89564-115">The state of the policy.</span></span> <span data-ttu-id="89564-116">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="89564-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89564-117">Связи</span><span class="sxs-lookup"><span data-stu-id="89564-117">Relationships</span></span>
<span data-ttu-id="89564-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89564-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89564-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89564-119">JSON representation</span></span>
<span data-ttu-id="89564-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89564-120">The following is a JSON representation of the resource.</span></span>
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
