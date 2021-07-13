---
title: тип ресурса managedTenantOperationError
description: Абстрактный тип, который представляет ошибку для управляемой операции клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d8dc51747ac63f6f8a719b0256c398d14d1c4034
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403045"
---
# <a name="managedtenantoperationerror-resource-type"></a><span data-ttu-id="0c6b7-103">тип ресурса managedTenantOperationError</span><span class="sxs-lookup"><span data-stu-id="0c6b7-103">managedTenantOperationError resource type</span></span>

<span data-ttu-id="0c6b7-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0c6b7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c6b7-105">Абстрактный тип, который представляет ошибку для управляемой операции клиента.</span><span class="sxs-lookup"><span data-stu-id="0c6b7-105">An abstract type that represents an error for a managed tenant operation.</span></span>

## <a name="properties"></a><span data-ttu-id="0c6b7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c6b7-106">Properties</span></span>
|<span data-ttu-id="0c6b7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c6b7-107">Property</span></span>|<span data-ttu-id="0c6b7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0c6b7-108">Type</span></span>|<span data-ttu-id="0c6b7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0c6b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c6b7-110">error</span><span class="sxs-lookup"><span data-stu-id="0c6b7-110">error</span></span>|<span data-ttu-id="0c6b7-111">String</span><span class="sxs-lookup"><span data-stu-id="0c6b7-111">String</span></span>|<span data-ttu-id="0c6b7-112">Сообщение об ошибке для исключения.</span><span class="sxs-lookup"><span data-stu-id="0c6b7-112">The error message for the exception.</span></span>|
|<span data-ttu-id="0c6b7-113">tenantId</span><span class="sxs-lookup"><span data-stu-id="0c6b7-113">tenantId</span></span>|<span data-ttu-id="0c6b7-114">String</span><span class="sxs-lookup"><span data-stu-id="0c6b7-114">String</span></span>|<span data-ttu-id="0c6b7-115">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="0c6b7-115">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c6b7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0c6b7-116">Relationships</span></span>
<span data-ttu-id="0c6b7-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0c6b7-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c6b7-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0c6b7-118">JSON representation</span></span>
<span data-ttu-id="0c6b7-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c6b7-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantOperationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantOperationError",
  "tenantId": "String",
  "error": "String"
}
```
