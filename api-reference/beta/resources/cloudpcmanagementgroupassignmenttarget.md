---
title: Тип ресурса Клаудпкманажементграупассигнменттаржет
description: 'Сложный тип, представляющий целевую группу назначения. Базовый тип: Клаудпкманажементассигнменттаржет'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378637"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="0f387-104">Тип ресурса Клаудпкманажементграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="0f387-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="0f387-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f387-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f387-106">Сложный тип, представляющий целевую группу назначения.</span><span class="sxs-lookup"><span data-stu-id="0f387-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="0f387-107">Наследуется от [клаудпкманажементассигнменттаржет](../resources/cloudpcmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="0f387-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0f387-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f387-108">Properties</span></span>

|<span data-ttu-id="0f387-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f387-109">Property</span></span>|<span data-ttu-id="0f387-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f387-110">Type</span></span>|<span data-ttu-id="0f387-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f387-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f387-112">groupId</span><span class="sxs-lookup"><span data-stu-id="0f387-112">groupId</span></span>|<span data-ttu-id="0f387-113">String</span><span class="sxs-lookup"><span data-stu-id="0f387-113">String</span></span>|<span data-ttu-id="0f387-114">Идентификатор целевой группы назначения</span><span class="sxs-lookup"><span data-stu-id="0f387-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f387-115">Связи</span><span class="sxs-lookup"><span data-stu-id="0f387-115">Relationships</span></span>

<span data-ttu-id="0f387-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0f387-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f387-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f387-117">JSON representation</span></span>

<span data-ttu-id="0f387-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f387-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
