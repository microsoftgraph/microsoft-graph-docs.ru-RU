---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd925db9eef2c03702ded5927408c6fc2d6ef399
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026749"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="0cc02-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="0cc02-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="0cc02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cc02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cc02-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cc02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc02-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cc02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc02-107">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cc02-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="0cc02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cc02-108">Properties</span></span>
|<span data-ttu-id="0cc02-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cc02-109">Property</span></span>|<span data-ttu-id="0cc02-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0cc02-110">Type</span></span>|<span data-ttu-id="0cc02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc02-112">name</span><span class="sxs-lookup"><span data-stu-id="0cc02-112">name</span></span>|<span data-ttu-id="0cc02-113">String</span><span class="sxs-lookup"><span data-stu-id="0cc02-113">String</span></span>|<span data-ttu-id="0cc02-114">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="0cc02-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="0cc02-115">description</span><span class="sxs-lookup"><span data-stu-id="0cc02-115">description</span></span>|<span data-ttu-id="0cc02-116">String</span><span class="sxs-lookup"><span data-stu-id="0cc02-116">String</span></span>|<span data-ttu-id="0cc02-117">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="0cc02-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="0cc02-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="0cc02-118">securityIdentifier</span></span>|<span data-ttu-id="0cc02-119">String</span><span class="sxs-lookup"><span data-stu-id="0cc02-119">String</span></span>|<span data-ttu-id="0cc02-120">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="0cc02-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cc02-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="0cc02-121">Relationships</span></span>
<span data-ttu-id="0cc02-122">Нет</span><span class="sxs-lookup"><span data-stu-id="0cc02-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cc02-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cc02-123">JSON Representation</span></span>
<span data-ttu-id="0cc02-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cc02-124">Here is a JSON representation of the resource.</span></span>
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






