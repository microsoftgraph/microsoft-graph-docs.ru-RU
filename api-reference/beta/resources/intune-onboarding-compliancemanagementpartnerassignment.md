---
title: Тип ресурса Комплианцеманажементпартнерассигнмент
description: Нацеленность для группы пользователей для партнера по управлению соответствием требованиям
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a04caf164e6761c95676b9029a2533cd86e7370
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524204"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a><span data-ttu-id="de1ec-103">Тип ресурса Комплианцеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="de1ec-103">complianceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="de1ec-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de1ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de1ec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de1ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de1ec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de1ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de1ec-107">Нацеленность для группы пользователей для партнера по управлению соответствием требованиям</span><span class="sxs-lookup"><span data-stu-id="de1ec-107">User group targeting for Compliance Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="de1ec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de1ec-108">Properties</span></span>
|<span data-ttu-id="de1ec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de1ec-109">Property</span></span>|<span data-ttu-id="de1ec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de1ec-110">Type</span></span>|<span data-ttu-id="de1ec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de1ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de1ec-112">target</span><span class="sxs-lookup"><span data-stu-id="de1ec-112">target</span></span>|[<span data-ttu-id="de1ec-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de1ec-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de1ec-114">Целевой объект назначения группы.</span><span class="sxs-lookup"><span data-stu-id="de1ec-114">Group assignment target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de1ec-115">Связи</span><span class="sxs-lookup"><span data-stu-id="de1ec-115">Relationships</span></span>
<span data-ttu-id="de1ec-116">Нет</span><span class="sxs-lookup"><span data-stu-id="de1ec-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de1ec-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de1ec-117">JSON Representation</span></span>
<span data-ttu-id="de1ec-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de1ec-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



