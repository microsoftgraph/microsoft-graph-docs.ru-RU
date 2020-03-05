---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5427be3bd28b46d18e4342e1731255c2675d910
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524120"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="33fef-103">Тип ресурса Девицеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="33fef-103">deviceManagementPartnerAssignment resource type</span></span>

<span data-ttu-id="33fef-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="33fef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33fef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33fef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33fef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33fef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33fef-107">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="33fef-107">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="33fef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="33fef-108">Properties</span></span>
|<span data-ttu-id="33fef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="33fef-109">Property</span></span>|<span data-ttu-id="33fef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="33fef-110">Type</span></span>|<span data-ttu-id="33fef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="33fef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33fef-112">target</span><span class="sxs-lookup"><span data-stu-id="33fef-112">target</span></span>|[<span data-ttu-id="33fef-113">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="33fef-113">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="33fef-114">Группы пользователей, предназначенные для регистрации устройств с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="33fef-114">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33fef-115">Связи</span><span class="sxs-lookup"><span data-stu-id="33fef-115">Relationships</span></span>
<span data-ttu-id="33fef-116">Нет</span><span class="sxs-lookup"><span data-stu-id="33fef-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33fef-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33fef-117">JSON Representation</span></span>
<span data-ttu-id="33fef-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33fef-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



