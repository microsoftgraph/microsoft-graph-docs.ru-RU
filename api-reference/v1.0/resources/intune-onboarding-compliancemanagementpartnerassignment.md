---
title: тип ресурса complianceManagementPartnerAssignment
description: Ориентация группы пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 638a50d7c8a6f1723c841c21f06d8cb44ac65460
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755653"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="a432a-103">тип ресурса complianceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="a432a-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="a432a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a432a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a432a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a432a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a432a-106">Ориентация группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="a432a-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="a432a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a432a-107">Properties</span></span>
|<span data-ttu-id="a432a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a432a-108">Property</span></span>|<span data-ttu-id="a432a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a432a-109">Type</span></span>|<span data-ttu-id="a432a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a432a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a432a-111">target</span><span class="sxs-lookup"><span data-stu-id="a432a-111">target</span></span>|[<span data-ttu-id="a432a-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a432a-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a432a-113">Цель группового назначения.</span><span class="sxs-lookup"><span data-stu-id="a432a-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a432a-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="a432a-114">Relationships</span></span>
<span data-ttu-id="a432a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a432a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a432a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a432a-116">JSON Representation</span></span>
<span data-ttu-id="a432a-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a432a-117">Here is a JSON representation of the resource.</span></span>
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
    "collectionId": "String"
  }
}
```




