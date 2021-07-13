---
title: тип ресурса managedTenantExecutionError
description: Представляет исключение для управляемой операции клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402429"
---
# <a name="managedtenantexecutionerror-resource-type"></a><span data-ttu-id="3327b-103">тип ресурса managedTenantExecutionError</span><span class="sxs-lookup"><span data-stu-id="3327b-103">managedTenantExecutionError resource type</span></span>

<span data-ttu-id="3327b-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3327b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3327b-105">Представляет исключение для управляемой операции клиента.</span><span class="sxs-lookup"><span data-stu-id="3327b-105">Represents an exception for a managed tenant operation.</span></span>

<span data-ttu-id="3327b-106">Наследует [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="3327b-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3327b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3327b-107">Properties</span></span>
|<span data-ttu-id="3327b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3327b-108">Property</span></span>|<span data-ttu-id="3327b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3327b-109">Type</span></span>|<span data-ttu-id="3327b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3327b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3327b-111">error</span><span class="sxs-lookup"><span data-stu-id="3327b-111">error</span></span>|<span data-ttu-id="3327b-112">String</span><span class="sxs-lookup"><span data-stu-id="3327b-112">String</span></span>|<span data-ttu-id="3327b-113">Сообщение об ошибке для исключения.</span><span class="sxs-lookup"><span data-stu-id="3327b-113">The error message for the exception.</span></span> <span data-ttu-id="3327b-114">Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="3327b-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="3327b-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3327b-115">Required.</span></span> <span data-ttu-id="3327b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-116">Read-only.</span></span>|
|<span data-ttu-id="3327b-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="3327b-117">errorDetails</span></span>|<span data-ttu-id="3327b-118">String</span><span class="sxs-lookup"><span data-stu-id="3327b-118">String</span></span>|<span data-ttu-id="3327b-119">Дополнительные сведения об ошибках для исключения.</span><span class="sxs-lookup"><span data-stu-id="3327b-119">Additional error information for the exception.</span></span> <span data-ttu-id="3327b-120">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3327b-120">Optional.</span></span> <span data-ttu-id="3327b-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-121">Read-only.</span></span>|
|<span data-ttu-id="3327b-122">nodeId</span><span class="sxs-lookup"><span data-stu-id="3327b-122">nodeId</span></span>|<span data-ttu-id="3327b-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3327b-123">Int32</span></span>|<span data-ttu-id="3327b-124">Идентификатор узла, в котором произошло исключение.</span><span class="sxs-lookup"><span data-stu-id="3327b-124">The node identifier where the exception occurred.</span></span> <span data-ttu-id="3327b-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3327b-125">Required.</span></span> <span data-ttu-id="3327b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-126">Read-only.</span></span>|
|<span data-ttu-id="3327b-127">rawToken</span><span class="sxs-lookup"><span data-stu-id="3327b-127">rawToken</span></span>|<span data-ttu-id="3327b-128">String</span><span class="sxs-lookup"><span data-stu-id="3327b-128">String</span></span>|<span data-ttu-id="3327b-129">Маркер для исключения.</span><span class="sxs-lookup"><span data-stu-id="3327b-129">The token for the exception.</span></span> <span data-ttu-id="3327b-130">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3327b-130">Optional.</span></span> <span data-ttu-id="3327b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-131">Read-only.</span></span>|
|<span data-ttu-id="3327b-132">statementIndex</span><span class="sxs-lookup"><span data-stu-id="3327b-132">statementIndex</span></span>|<span data-ttu-id="3327b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3327b-133">Int32</span></span>|<span data-ttu-id="3327b-134">Индекс заявления для исключения.</span><span class="sxs-lookup"><span data-stu-id="3327b-134">The statement index for the exception.</span></span> <span data-ttu-id="3327b-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3327b-135">Required.</span></span> <span data-ttu-id="3327b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-136">Read-only.</span></span>|
|<span data-ttu-id="3327b-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="3327b-137">tenantId</span></span>|<span data-ttu-id="3327b-138">String</span><span class="sxs-lookup"><span data-stu-id="3327b-138">String</span></span>|<span data-ttu-id="3327b-139">Идентификатор Azure Active Directory клиента для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="3327b-139">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="3327b-140">Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span><span class="sxs-lookup"><span data-stu-id="3327b-140">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="3327b-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3327b-141">Required.</span></span> <span data-ttu-id="3327b-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3327b-142">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3327b-143">Связи</span><span class="sxs-lookup"><span data-stu-id="3327b-143">Relationships</span></span>
<span data-ttu-id="3327b-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3327b-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3327b-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3327b-145">JSON representation</span></span>
<span data-ttu-id="3327b-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3327b-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
