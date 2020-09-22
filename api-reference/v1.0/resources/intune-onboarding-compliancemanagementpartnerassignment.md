---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9bdcfd0edcdf4e93b3bf11f8d30a3cef5cc9d60
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072972"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="7bbf1-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="7bbf1-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="7bbf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bbf1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bbf1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bbf1-106">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="7bbf1-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="7bbf1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bbf1-107">Properties</span></span>
|<span data-ttu-id="7bbf1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bbf1-108">Property</span></span>|<span data-ttu-id="7bbf1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7bbf1-109">Type</span></span>|<span data-ttu-id="7bbf1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7bbf1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bbf1-111">target</span><span class="sxs-lookup"><span data-stu-id="7bbf1-111">target</span></span>|[<span data-ttu-id="7bbf1-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7bbf1-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7bbf1-113">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="7bbf1-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bbf1-114">Связи</span><span class="sxs-lookup"><span data-stu-id="7bbf1-114">Relationships</span></span>
<span data-ttu-id="7bbf1-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7bbf1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bbf1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bbf1-116">JSON Representation</span></span>
<span data-ttu-id="7bbf1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bbf1-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```





