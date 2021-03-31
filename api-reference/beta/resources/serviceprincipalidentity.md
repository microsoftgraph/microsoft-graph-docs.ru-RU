---
title: тип ресурса servicePrincipalIdentity
description: Модели основного удостоверения службы.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a49adab87ac5ebe7b8eddf106d8d38c4e15acd11
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469786"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="c12e8-103">тип ресурса servicePrincipalIdentity</span><span class="sxs-lookup"><span data-stu-id="c12e8-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="c12e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c12e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c12e8-105">Модели основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="c12e8-105">Models a service principal identity.</span></span>

<span data-ttu-id="c12e8-106">Наследует от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c12e8-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c12e8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c12e8-107">Properties</span></span>
|<span data-ttu-id="c12e8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c12e8-108">Property</span></span>|<span data-ttu-id="c12e8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c12e8-109">Type</span></span>|<span data-ttu-id="c12e8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c12e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c12e8-111">appId</span><span class="sxs-lookup"><span data-stu-id="c12e8-111">appId</span></span>|<span data-ttu-id="c12e8-112">String</span><span class="sxs-lookup"><span data-stu-id="c12e8-112">String</span></span>| <span data-ttu-id="c12e8-113">Идентификатор приложения для директора службы.</span><span class="sxs-lookup"><span data-stu-id="c12e8-113">The application identifier of the service principal.</span></span> |
|<span data-ttu-id="c12e8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c12e8-114">displayName</span></span>|<span data-ttu-id="c12e8-115">String</span><span class="sxs-lookup"><span data-stu-id="c12e8-115">String</span></span>| <span data-ttu-id="c12e8-116">Отображение имени основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="c12e8-116">The display name of the service principal identity.</span></span> <span data-ttu-id="c12e8-117">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c12e8-117">Inherited from [identity](../resources/identity.md).</span></span> |
|<span data-ttu-id="c12e8-118">id</span><span class="sxs-lookup"><span data-stu-id="c12e8-118">id</span></span>|<span data-ttu-id="c12e8-119">String</span><span class="sxs-lookup"><span data-stu-id="c12e8-119">String</span></span>| <span data-ttu-id="c12e8-120">Идентификатор основного удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="c12e8-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="c12e8-121">Унаследованный от [удостоверения](../resources/identity.md).</span><span class="sxs-lookup"><span data-stu-id="c12e8-121">Inherited from [identity](../resources/identity.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c12e8-122">Связи</span><span class="sxs-lookup"><span data-stu-id="c12e8-122">Relationships</span></span>
<span data-ttu-id="c12e8-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c12e8-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c12e8-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c12e8-124">JSON representation</span></span>
<span data-ttu-id="c12e8-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c12e8-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
