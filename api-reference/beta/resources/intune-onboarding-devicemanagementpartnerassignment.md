---
title: Тип ресурса Девицеманажементпартнерассигнмент
description: Целевая группа пользователей для партнера по управлению устройствами
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 306acfae948a81ca5c8933f455a21347bf27ee9e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778724"
---
# <a name="devicemanagementpartnerassignment-resource-type"></a><span data-ttu-id="b1615-103">Тип ресурса Девицеманажементпартнерассигнмент</span><span class="sxs-lookup"><span data-stu-id="b1615-103">deviceManagementPartnerAssignment resource type</span></span>

> <span data-ttu-id="b1615-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1615-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1615-106">Целевая группа пользователей для партнера по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="b1615-106">User group targeting for Device Management Partner</span></span>

## <a name="properties"></a><span data-ttu-id="b1615-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1615-107">Properties</span></span>
|<span data-ttu-id="b1615-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1615-108">Property</span></span>|<span data-ttu-id="b1615-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b1615-109">Type</span></span>|<span data-ttu-id="b1615-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1615-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1615-111">target</span><span class="sxs-lookup"><span data-stu-id="b1615-111">target</span></span>|[<span data-ttu-id="b1615-112">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b1615-112">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b1615-113">Группы пользователей, предназначенные для регистрации устройств с помощью партнера.</span><span class="sxs-lookup"><span data-stu-id="b1615-113">User groups targeting for devices to be enrolled through partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1615-114">Связи</span><span class="sxs-lookup"><span data-stu-id="b1615-114">Relationships</span></span>
<span data-ttu-id="b1615-115">Нет</span><span class="sxs-lookup"><span data-stu-id="b1615-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1615-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1615-116">JSON Representation</span></span>
<span data-ttu-id="b1615-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1615-117">Here is a JSON representation of the resource.</span></span>
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



