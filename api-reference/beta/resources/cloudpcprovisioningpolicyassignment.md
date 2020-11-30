---
title: Тип ресурса Клаудпкпровисионингполициассигнмент
description: Назначения политик подготовки Клаудпк
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbbdf76dfb184efdae7279b5d4970367995c0a6c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378566"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a><span data-ttu-id="460d7-103">Тип ресурса Клаудпкпровисионингполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="460d7-103">cloudPcProvisioningPolicyAssignment resource type</span></span>

<span data-ttu-id="460d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="460d7-105">Представляет определенную коллекцию назначений политик подготовки.</span><span class="sxs-lookup"><span data-stu-id="460d7-105">Represents a defined collection of provisioning policy assignments.</span></span>


## <a name="properties"></a><span data-ttu-id="460d7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="460d7-106">Properties</span></span>

|<span data-ttu-id="460d7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="460d7-107">Property</span></span>|<span data-ttu-id="460d7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="460d7-108">Type</span></span>|<span data-ttu-id="460d7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="460d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460d7-110">id</span><span class="sxs-lookup"><span data-stu-id="460d7-110">id</span></span>|<span data-ttu-id="460d7-111">Строка</span><span class="sxs-lookup"><span data-stu-id="460d7-111">String</span></span>|<span data-ttu-id="460d7-112">Уникальный идентификатор назначения политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="460d7-112">Unique Identifier for the provisioning policy assignment.</span></span> <span data-ttu-id="460d7-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="460d7-113">Read-only.</span></span> <span data-ttu-id="460d7-114">Если `target` это группа пользователей, идентификатор отображается как {полициид} _ {groupId}.</span><span class="sxs-lookup"><span data-stu-id="460d7-114">If `target` is a user group, then the ID is shown as {policyId}_{groupId}.</span></span>|
|<span data-ttu-id="460d7-115">target</span><span class="sxs-lookup"><span data-stu-id="460d7-115">target</span></span>|[<span data-ttu-id="460d7-116">клаудпкманажементассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="460d7-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="460d7-117">Цель назначения для политики подготовки.</span><span class="sxs-lookup"><span data-stu-id="460d7-117">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="460d7-118">В настоящее время для этой политики поддерживается только одна цель — группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="460d7-118">Currently, the only target supported for this policy is a user group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="460d7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="460d7-119">Relationships</span></span>

<span data-ttu-id="460d7-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="460d7-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="460d7-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="460d7-121">JSON representation</span></span>

<span data-ttu-id="460d7-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="460d7-122">The following is a JSON representation of the resource.</span></span>
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
