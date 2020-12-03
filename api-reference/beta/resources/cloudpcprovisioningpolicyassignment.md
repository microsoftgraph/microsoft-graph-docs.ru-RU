---
title: Тип ресурса Клаудпкпровисионингполициассигнмент
description: Назначения политик подготовки Клаудпк
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563718"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="411ef-103">Тип ресурса Клаудпкпровисионингполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="411ef-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="411ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="411ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="411ef-105">Представляет определенную коллекцию назначений политик подготовки.</span><span class="sxs-lookup"><span data-stu-id="411ef-105">Represents a defined collection of provisioning policy assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="411ef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="411ef-106">Properties</span></span>

|<span data-ttu-id="411ef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="411ef-107">Property</span></span>|<span data-ttu-id="411ef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="411ef-108">Type</span></span>|<span data-ttu-id="411ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="411ef-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="411ef-110">id</span><span class="sxs-lookup"><span data-stu-id="411ef-110">id</span></span>|<span data-ttu-id="411ef-111">String</span><span class="sxs-lookup"><span data-stu-id="411ef-111">String</span></span>|<span data-ttu-id="411ef-112">Уникальный идентификатор назначения политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="411ef-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="411ef-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="411ef-113">Read-only.</span></span> <span data-ttu-id="411ef-114">Если `target` это группа пользователей, идентификатор отображается как {полициид} _ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="411ef-114">If `target` is a user group, then the ID is shown as {policyId}_{groupId}.</span></span>|
|<span data-ttu-id="411ef-115">target</span><span class="sxs-lookup"><span data-stu-id="411ef-115">target</span></span>|[<span data-ttu-id="411ef-116">клаудпкманажементассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="411ef-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="411ef-117">Цель назначения для политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="411ef-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="411ef-118">В настоящее время для этой политики поддерживается только одна цель — группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="411ef-118">Currently, the only target supported for this policy is a user group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="411ef-119">Связи</span><span class="sxs-lookup"><span data-stu-id="411ef-119">Relationships</span></span>

<span data-ttu-id="411ef-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="411ef-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="411ef-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="411ef-121">JSON representation</span></span>

<span data-ttu-id="411ef-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="411ef-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
