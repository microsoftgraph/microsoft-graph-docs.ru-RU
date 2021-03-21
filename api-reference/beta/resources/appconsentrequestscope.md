---
title: тип ресурса appConsentRequestScope
description: Сведения о динамических области разрешений, для которых запрашивается доступ.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b960820e0d7cf20a37850256bb96ba3abf034038
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965232"
---
# <a name="appconsentrequestscope-resource-type"></a><span data-ttu-id="e0f62-103">тип ресурса appConsentRequestScope</span><span class="sxs-lookup"><span data-stu-id="e0f62-103">appConsentRequestScope resource type</span></span>

<span data-ttu-id="e0f62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0f62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0f62-105">В **appConsentRequestScope** подробно извещаются динамические области разрешений, для которых запрашивается доступ.</span><span class="sxs-lookup"><span data-stu-id="e0f62-105">The **appConsentRequestScope** details the dynamic permission scopes for which access is being requested.</span></span>

## <a name="properties"></a><span data-ttu-id="e0f62-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0f62-106">Properties</span></span>
|<span data-ttu-id="e0f62-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0f62-107">Property</span></span>|<span data-ttu-id="e0f62-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e0f62-108">Type</span></span>|<span data-ttu-id="e0f62-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f62-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0f62-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e0f62-110">displayName</span></span>|<span data-ttu-id="e0f62-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e0f62-111">String</span></span>|<span data-ttu-id="e0f62-112">Имя области.</span><span class="sxs-lookup"><span data-stu-id="e0f62-112">The name of the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0f62-113">Связи</span><span class="sxs-lookup"><span data-stu-id="e0f62-113">Relationships</span></span>
<span data-ttu-id="e0f62-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e0f62-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0f62-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0f62-115">JSON representation</span></span>
<span data-ttu-id="e0f62-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f62-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConsentRequestScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequestScope",
  "displayName": "String"
}
```

