---
title: Тип ресурса deviceManagementPartnerAssignment
description: Целевая группа пользователей для партнера по управлению устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0cda49b654313ec4d69e810033ae681b8ac2645
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157542"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="012a1-103">Тип ресурса deviceManagementPartnerAssignment</span><span class="sxs-lookup"><span data-stu-id="012a1-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="012a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="012a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="012a1-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="012a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="012a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="012a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="012a1-107">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="012a1-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="012a1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="012a1-108">Properties</span></span>
|<span data-ttu-id="012a1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="012a1-109">Property</span></span>|<span data-ttu-id="012a1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="012a1-110">Type</span></span>|<span data-ttu-id="012a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="012a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="012a1-112">target</span><span class="sxs-lookup"><span data-stu-id="012a1-112">target</span></span>|[<span data-ttu-id="012a1-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="012a1-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="012a1-114">Группы пользователей, нацеленные на регистрацию устройств через партнера.</span><span class="sxs-lookup"><span data-stu-id="012a1-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="012a1-115">Связи</span><span class="sxs-lookup"><span data-stu-id="012a1-115">Relationships</span></span>
<span data-ttu-id="012a1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="012a1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="012a1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="012a1-117">JSON Representation</span></span>
<span data-ttu-id="012a1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="012a1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




