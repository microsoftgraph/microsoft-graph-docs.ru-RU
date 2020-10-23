---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf4d5ebcd77dfef119d97e0d5bbe2bfbfb93c4e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707817"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d329e-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="d329e-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="d329e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d329e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d329e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d329e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d329e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d329e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d329e-107">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="d329e-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="d329e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d329e-108">Properties</span></span>
|<span data-ttu-id="d329e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d329e-109">Property</span></span>|<span data-ttu-id="d329e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d329e-110">Type</span></span>|<span data-ttu-id="d329e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d329e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d329e-112">name</span><span class="sxs-lookup"><span data-stu-id="d329e-112">name</span></span>|<span data-ttu-id="d329e-113">String</span><span class="sxs-lookup"><span data-stu-id="d329e-113">String</span></span>|<span data-ttu-id="d329e-114">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d329e-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="d329e-115">description</span><span class="sxs-lookup"><span data-stu-id="d329e-115">description</span></span>|<span data-ttu-id="d329e-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d329e-116">String</span></span>|<span data-ttu-id="d329e-117">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="d329e-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d329e-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d329e-118">securityIdentifier</span></span>|<span data-ttu-id="d329e-119">String</span><span class="sxs-lookup"><span data-stu-id="d329e-119">String</span></span>|<span data-ttu-id="d329e-120">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d329e-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d329e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d329e-121">Relationships</span></span>
<span data-ttu-id="d329e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d329e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d329e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d329e-123">JSON Representation</span></span>
<span data-ttu-id="d329e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d329e-124">Here is a JSON representation of the resource.</span></span>
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





