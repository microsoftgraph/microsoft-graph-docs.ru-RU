---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 49721c0713bcb2b2af7b3b19fbcb3c2f4a816194
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792005"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="74be8-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="74be8-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="74be8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74be8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74be8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74be8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74be8-106">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="74be8-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="74be8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74be8-107">Properties</span></span>
|<span data-ttu-id="74be8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74be8-108">Property</span></span>|<span data-ttu-id="74be8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74be8-109">Type</span></span>|<span data-ttu-id="74be8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74be8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74be8-111">name</span><span class="sxs-lookup"><span data-stu-id="74be8-111">name</span></span>|<span data-ttu-id="74be8-112">String</span><span class="sxs-lookup"><span data-stu-id="74be8-112">String</span></span>|<span data-ttu-id="74be8-113">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="74be8-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="74be8-114">description</span><span class="sxs-lookup"><span data-stu-id="74be8-114">description</span></span>|<span data-ttu-id="74be8-115">String</span><span class="sxs-lookup"><span data-stu-id="74be8-115">String</span></span>|<span data-ttu-id="74be8-116">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="74be8-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="74be8-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="74be8-117">securityIdentifier</span></span>|<span data-ttu-id="74be8-118">String</span><span class="sxs-lookup"><span data-stu-id="74be8-118">String</span></span>|<span data-ttu-id="74be8-119">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="74be8-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="74be8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="74be8-120">Relationships</span></span>
<span data-ttu-id="74be8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="74be8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74be8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74be8-122">JSON Representation</span></span>
<span data-ttu-id="74be8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74be8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```



