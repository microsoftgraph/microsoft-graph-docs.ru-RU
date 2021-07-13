---
title: тип ресурса managedTenantGenericError
description: Представляет общую ошибку для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402411"
---
# <a name="managedtenantgenericerror-resource-type"></a><span data-ttu-id="d8e85-103">тип ресурса managedTenantGenericError</span><span class="sxs-lookup"><span data-stu-id="d8e85-103">managedTenantGenericError resource type</span></span>

<span data-ttu-id="d8e85-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d8e85-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8e85-105">Представляет общую ошибку для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="d8e85-105">Represents a generic error for a managed tenant.</span></span>

<span data-ttu-id="d8e85-106">Наследует [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="d8e85-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d8e85-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8e85-107">Properties</span></span>
|<span data-ttu-id="d8e85-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8e85-108">Property</span></span>|<span data-ttu-id="d8e85-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d8e85-109">Type</span></span>|<span data-ttu-id="d8e85-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d8e85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e85-111">error</span><span class="sxs-lookup"><span data-stu-id="d8e85-111">error</span></span>|<span data-ttu-id="d8e85-112">String</span><span class="sxs-lookup"><span data-stu-id="d8e85-112">String</span></span>|<span data-ttu-id="d8e85-113">Сообщение об ошибке для исключения.</span><span class="sxs-lookup"><span data-stu-id="d8e85-113">The error message for the exception.</span></span> <span data-ttu-id="d8e85-114">Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="d8e85-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="d8e85-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8e85-115">Required.</span></span> <span data-ttu-id="d8e85-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8e85-116">Read-only.</span></span>|
|<span data-ttu-id="d8e85-117">tenantId</span><span class="sxs-lookup"><span data-stu-id="d8e85-117">tenantId</span></span>|<span data-ttu-id="d8e85-118">String</span><span class="sxs-lookup"><span data-stu-id="d8e85-118">String</span></span>|<span data-ttu-id="d8e85-119">Идентификатор Azure Active Directory клиента для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="d8e85-119">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="d8e85-120">Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="d8e85-120">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="d8e85-121">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d8e85-121">Optional.</span></span> <span data-ttu-id="d8e85-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8e85-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8e85-123">Связи</span><span class="sxs-lookup"><span data-stu-id="d8e85-123">Relationships</span></span>
<span data-ttu-id="d8e85-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8e85-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8e85-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d8e85-125">JSON representation</span></span>
<span data-ttu-id="d8e85-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8e85-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
