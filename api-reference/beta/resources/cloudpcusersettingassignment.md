---
title: тип ресурса cloudPcUserSettingAssignment
description: Представляет определенный набор назначений параметров пользователя.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 704142ce266a826606b6c32b209d69d052d1a3c9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993739"
---
# <a name="cloudpcusersettingassignment--resource-type"></a><span data-ttu-id="03e8d-103">тип ресурса cloudPcUserSettingAssignment</span><span class="sxs-lookup"><span data-stu-id="03e8d-103">cloudPcUserSettingAssignment  resource type</span></span>

<span data-ttu-id="03e8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03e8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03e8d-105">Представляет определенный набор назначений параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="03e8d-105">Represents a defined collection of user setting assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="03e8d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="03e8d-106">Properties</span></span>

|<span data-ttu-id="03e8d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="03e8d-107">Property</span></span>|<span data-ttu-id="03e8d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="03e8d-108">Type</span></span>|<span data-ttu-id="03e8d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="03e8d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e8d-110">id</span><span class="sxs-lookup"><span data-stu-id="03e8d-110">id</span></span>|<span data-ttu-id="03e8d-111">String</span><span class="sxs-lookup"><span data-stu-id="03e8d-111">String</span></span>|<span data-ttu-id="03e8d-112">Уникальный идентификатор для назначения настройки пользователя.</span><span class="sxs-lookup"><span data-stu-id="03e8d-112">Unique Identifier for the user setting assignment.</span></span> <span data-ttu-id="03e8d-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03e8d-113">Read-only.</span></span> <span data-ttu-id="03e8d-114">Если `target` это группа пользователей, у ID есть эта структура: {policyID}_{groupID}.</span><span class="sxs-lookup"><span data-stu-id="03e8d-114">If `target` is a user group, the ID has this structure: {policyID}_{groupID}.</span></span>|
|<span data-ttu-id="03e8d-115">target</span><span class="sxs-lookup"><span data-stu-id="03e8d-115">target</span></span>|[<span data-ttu-id="03e8d-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="03e8d-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="03e8d-117">Цель назначения для параметра пользователя.</span><span class="sxs-lookup"><span data-stu-id="03e8d-117">The assignment target for the user setting.</span></span> <span data-ttu-id="03e8d-118">В настоящее время единственной целевой целью, поддерживаемой для параметров пользователя, является группа пользователей.</span><span class="sxs-lookup"><span data-stu-id="03e8d-118">Currently, the only target supported for user setting is a user group.</span></span>|
|<span data-ttu-id="03e8d-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03e8d-119">createdDateTime</span></span>|<span data-ttu-id="03e8d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e8d-120">DateTimeOffset</span></span>|<span data-ttu-id="03e8d-121">Дата и время создания этого назначения.</span><span class="sxs-lookup"><span data-stu-id="03e8d-121">The date and time this assignment was created.</span></span> <span data-ttu-id="03e8d-122">Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="03e8d-122">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03e8d-123">Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="03e8d-123">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="03e8d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="03e8d-124">Relationships</span></span>

<span data-ttu-id="03e8d-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="03e8d-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03e8d-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="03e8d-126">JSON representation</span></span>
<span data-ttu-id="03e8d-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03e8d-127">The following is a JSON representation of the resource.</span></span>
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
