---
title: тип ресурса appConsentRequestScope
description: Сведения о динамических области разрешений, для которых запрашивается доступ.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 644ce45997d155a8c3a0bc893af910301e5ba22c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469702"
---
# <a name="appconsentrequestscope-resource-type"></a><span data-ttu-id="3da1f-103">тип ресурса appConsentRequestScope</span><span class="sxs-lookup"><span data-stu-id="3da1f-103">appConsentRequestScope resource type</span></span>

<span data-ttu-id="3da1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da1f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3da1f-105">В **appConsentRequestScope** подробно извещаются динамические области разрешений, для которых запрашивается доступ.</span><span class="sxs-lookup"><span data-stu-id="3da1f-105">The **appConsentRequestScope** details the dynamic permission scopes for which access is being requested.</span></span>

## <a name="properties"></a><span data-ttu-id="3da1f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3da1f-106">Properties</span></span>

|<span data-ttu-id="3da1f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3da1f-107">Property</span></span>|<span data-ttu-id="3da1f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3da1f-108">Type</span></span>|<span data-ttu-id="3da1f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3da1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da1f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3da1f-110">displayName</span></span>|<span data-ttu-id="3da1f-111">String</span><span class="sxs-lookup"><span data-stu-id="3da1f-111">String</span></span>|<span data-ttu-id="3da1f-112">Имя области.</span><span class="sxs-lookup"><span data-stu-id="3da1f-112">The name of the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3da1f-113">Связи</span><span class="sxs-lookup"><span data-stu-id="3da1f-113">Relationships</span></span>

<span data-ttu-id="3da1f-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3da1f-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3da1f-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3da1f-115">JSON representation</span></span>

<span data-ttu-id="3da1f-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3da1f-116">The following is a JSON representation of the resource.</span></span>
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

