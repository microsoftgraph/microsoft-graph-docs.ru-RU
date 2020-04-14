---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f17c22d8719f60ee28732727607db62422f1b74b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469248"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="58c49-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="58c49-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="58c49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58c49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58c49-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58c49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58c49-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58c49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c49-107">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="58c49-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="58c49-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="58c49-108">Properties</span></span>
|<span data-ttu-id="58c49-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="58c49-109">Property</span></span>|<span data-ttu-id="58c49-110">Тип</span><span class="sxs-lookup"><span data-stu-id="58c49-110">Type</span></span>|<span data-ttu-id="58c49-111">Описание</span><span class="sxs-lookup"><span data-stu-id="58c49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c49-112">name</span><span class="sxs-lookup"><span data-stu-id="58c49-112">name</span></span>|<span data-ttu-id="58c49-113">String</span><span class="sxs-lookup"><span data-stu-id="58c49-113">String</span></span>|<span data-ttu-id="58c49-114">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="58c49-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="58c49-115">description</span><span class="sxs-lookup"><span data-stu-id="58c49-115">description</span></span>|<span data-ttu-id="58c49-116">String</span><span class="sxs-lookup"><span data-stu-id="58c49-116">String</span></span>|<span data-ttu-id="58c49-117">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="58c49-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="58c49-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="58c49-118">securityIdentifier</span></span>|<span data-ttu-id="58c49-119">String</span><span class="sxs-lookup"><span data-stu-id="58c49-119">String</span></span>|<span data-ttu-id="58c49-120">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="58c49-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="58c49-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="58c49-121">Relationships</span></span>
<span data-ttu-id="58c49-122">Нет</span><span class="sxs-lookup"><span data-stu-id="58c49-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58c49-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58c49-123">JSON Representation</span></span>
<span data-ttu-id="58c49-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58c49-124">Here is a JSON representation of the resource.</span></span>
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



