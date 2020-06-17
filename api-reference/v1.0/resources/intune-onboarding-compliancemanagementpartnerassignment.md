---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf246cd1f7fad0d168165f72a3861005e8cefbe
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744167"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="b11a7-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="b11a7-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="b11a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b11a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b11a7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b11a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b11a7-106">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="b11a7-106">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="b11a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b11a7-107">Properties</span></span>
|<span data-ttu-id="b11a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b11a7-108">Property</span></span>|<span data-ttu-id="b11a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b11a7-109">Type</span></span>|<span data-ttu-id="b11a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b11a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b11a7-111">target</span><span class="sxs-lookup"><span data-stu-id="b11a7-111">target</span></span>|[<span data-ttu-id="b11a7-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b11a7-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b11a7-113">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="b11a7-113">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b11a7-114">Связи</span><span class="sxs-lookup"><span data-stu-id="b11a7-114">Relationships</span></span>
<span data-ttu-id="b11a7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="b11a7-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b11a7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b11a7-116">JSON Representation</span></span>
<span data-ttu-id="b11a7-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b11a7-117">Here is a JSON representation of the resource.</span></span>
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



