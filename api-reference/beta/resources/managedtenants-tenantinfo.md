---
title: тип ресурса tenantInfo
description: Представляет сведения для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c81df716b74511daab1f713f73bdd872e84e4987
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402688"
---
# <a name="tenantinfo-resource-type"></a><span data-ttu-id="aef70-103">тип ресурса tenantInfo</span><span class="sxs-lookup"><span data-stu-id="aef70-103">tenantInfo resource type</span></span>

<span data-ttu-id="aef70-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="aef70-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aef70-105">Представляет сведения для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="aef70-105">Represents information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="aef70-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aef70-106">Properties</span></span>
|<span data-ttu-id="aef70-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="aef70-107">Property</span></span>|<span data-ttu-id="aef70-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aef70-108">Type</span></span>|<span data-ttu-id="aef70-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aef70-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef70-110">tenantId</span><span class="sxs-lookup"><span data-stu-id="aef70-110">tenantId</span></span>|<span data-ttu-id="aef70-111">String</span><span class="sxs-lookup"><span data-stu-id="aef70-111">String</span></span>|<span data-ttu-id="aef70-112">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="aef70-112">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="aef70-113">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="aef70-113">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aef70-114">Связи</span><span class="sxs-lookup"><span data-stu-id="aef70-114">Relationships</span></span>
<span data-ttu-id="aef70-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aef70-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aef70-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aef70-116">JSON representation</span></span>
<span data-ttu-id="aef70-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aef70-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantInfo",
  "tenantId": "String"
}
```
