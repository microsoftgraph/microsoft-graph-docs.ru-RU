---
title: Тип ресурса Клаудпкманажементграупассигнменттаржет
description: 'Сложный тип, представляющий целевую группу назначения. Базовый тип: Клаудпкманажементассигнменттаржет'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563874"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a><span data-ttu-id="bab7e-104">Тип ресурса Клаудпкманажементграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="bab7e-104">cloudPcManagementGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="bab7e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab7e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bab7e-106">Сложный тип, представляющий целевую группу назначения.</span><span class="sxs-lookup"><span data-stu-id="bab7e-106">Complex type that represents the assignment target group.</span></span>
<span data-ttu-id="bab7e-107">Наследуется от [клаудпкманажементассигнменттаржет](../resources/cloudpcmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="bab7e-107">Inherits from [cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="bab7e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bab7e-108">Properties</span></span>

|<span data-ttu-id="bab7e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bab7e-109">Property</span></span>|<span data-ttu-id="bab7e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bab7e-110">Type</span></span>|<span data-ttu-id="bab7e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bab7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bab7e-112">groupId</span><span class="sxs-lookup"><span data-stu-id="bab7e-112">groupId</span></span>|<span data-ttu-id="bab7e-113">String</span><span class="sxs-lookup"><span data-stu-id="bab7e-113">String</span></span>|<span data-ttu-id="bab7e-114">Идентификатор целевой группы назначения</span><span class="sxs-lookup"><span data-stu-id="bab7e-114">The id of the assignment's target group</span></span>|

## <a name="relationships"></a><span data-ttu-id="bab7e-115">Связи</span><span class="sxs-lookup"><span data-stu-id="bab7e-115">Relationships</span></span>

<span data-ttu-id="bab7e-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bab7e-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bab7e-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bab7e-117">JSON representation</span></span>

<span data-ttu-id="bab7e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bab7e-118">The following is a JSON representation of the resource.</span></span>
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
