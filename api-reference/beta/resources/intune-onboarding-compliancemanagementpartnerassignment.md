---
title: Тип ресурса complianceManagementPartnerAssignment
description: Целевая группа пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46e4e6a5e073e3087267329880cf0f36bb79c4a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161441"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="112b5-103">Тип ресурса complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="112b5-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="112b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="112b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="112b5-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="112b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="112b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="112b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="112b5-107">Целевая группа пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="112b5-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="112b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="112b5-108">Properties</span></span>
|<span data-ttu-id="112b5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="112b5-109">Property</span></span>|<span data-ttu-id="112b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="112b5-110">Type</span></span>|<span data-ttu-id="112b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="112b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="112b5-112">target</span><span class="sxs-lookup"><span data-stu-id="112b5-112">target</span></span>|[<span data-ttu-id="112b5-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="112b5-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="112b5-114">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="112b5-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="112b5-115">Связи</span><span class="sxs-lookup"><span data-stu-id="112b5-115">Relationships</span></span>
<span data-ttu-id="112b5-116">Нет</span><span class="sxs-lookup"><span data-stu-id="112b5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="112b5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="112b5-117">JSON Representation</span></span>
<span data-ttu-id="112b5-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="112b5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




