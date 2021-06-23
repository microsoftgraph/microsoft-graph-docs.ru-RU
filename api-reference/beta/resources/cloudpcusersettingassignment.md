---
title: тип ресурса cloudPcUserSettingAssignment
description: Представляет определенный набор назначений параметров пользователя.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db97ff52ff8eb7ca1ef52563d577d5076273d859
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082190"
---
# <a name="cloudpcusersettingassignment--resource-type"></a><span data-ttu-id="1a2e6-103">тип ресурса cloudPcUserSettingAssignment</span><span class="sxs-lookup"><span data-stu-id="1a2e6-103">cloudPcUserSettingAssignment  resource type</span></span>

<span data-ttu-id="1a2e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a2e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a2e6-105">Представляет определенный набор назначений параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-105">Represents a defined collection of user setting assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="1a2e6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a2e6-106">Properties</span></span>

|<span data-ttu-id="1a2e6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a2e6-107">Property</span></span>|<span data-ttu-id="1a2e6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1a2e6-108">Type</span></span>|<span data-ttu-id="1a2e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a2e6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a2e6-110">id</span><span class="sxs-lookup"><span data-stu-id="1a2e6-110">id</span></span>|<span data-ttu-id="1a2e6-111">String</span><span class="sxs-lookup"><span data-stu-id="1a2e6-111">String</span></span>|<span data-ttu-id="1a2e6-112">Уникальный идентификатор для назначения настройки пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-112">Unique Identifier for the user setting assignment.</span></span> <span data-ttu-id="1a2e6-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-113">Read-only.</span></span> <span data-ttu-id="1a2e6-114">Если `target` это группа пользователей, iD имеет эту структуру: {policyID} \_ {groupID}.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-114">If `target` is a user group, the ID has this structure: {policyID}\_{groupID}.</span></span>|
|<span data-ttu-id="1a2e6-115">target</span><span class="sxs-lookup"><span data-stu-id="1a2e6-115">target</span></span>|[<span data-ttu-id="1a2e6-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1a2e6-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="1a2e6-117">Цель назначения для параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-117">The assignment target for the user setting.</span></span> <span data-ttu-id="1a2e6-118">В настоящее время единственной целевой целью, поддерживаемой для этого параметра пользователя, является группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-118">Currently, the only target supported for this user setting is a user group.</span></span> <span data-ttu-id="1a2e6-119">Подробные сведения см. [в материале cloudPcManagementGroupAssignmentTarget.](cloudpcmanagementgroupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1a2e6-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span>|
|<span data-ttu-id="1a2e6-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2e6-120">createdDateTime</span></span>|<span data-ttu-id="1a2e6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2e6-121">DateTimeOffset</span></span>|<span data-ttu-id="1a2e6-122">Дата и время создания этого назначения.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-122">The date and time this assignment was created.</span></span> <span data-ttu-id="1a2e6-123">Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-123">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1a2e6-124">Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-124">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="1a2e6-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1a2e6-125">Relationships</span></span>

<span data-ttu-id="1a2e6-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a2e6-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a2e6-127">JSON representation</span></span>
<span data-ttu-id="1a2e6-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a2e6-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
