---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bf4ac6aa9de235b1e4117b47c6a5eafc5c011a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332752"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d1287-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="d1287-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="d1287-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1287-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1287-106">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1287-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="d1287-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1287-107">Properties</span></span>
|<span data-ttu-id="d1287-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1287-108">Property</span></span>|<span data-ttu-id="d1287-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d1287-109">Type</span></span>|<span data-ttu-id="d1287-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d1287-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1287-111">name</span><span class="sxs-lookup"><span data-stu-id="d1287-111">name</span></span>|<span data-ttu-id="d1287-112">String</span><span class="sxs-lookup"><span data-stu-id="d1287-112">String</span></span>|<span data-ttu-id="d1287-113">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d1287-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="d1287-114">description</span><span class="sxs-lookup"><span data-stu-id="d1287-114">description</span></span>|<span data-ttu-id="d1287-115">String</span><span class="sxs-lookup"><span data-stu-id="d1287-115">String</span></span>|<span data-ttu-id="d1287-116">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="d1287-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d1287-117">секуритидентифиер</span><span class="sxs-lookup"><span data-stu-id="d1287-117">securityIdentifier</span></span>|<span data-ttu-id="d1287-118">String</span><span class="sxs-lookup"><span data-stu-id="d1287-118">String</span></span>|<span data-ttu-id="d1287-119">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d1287-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1287-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1287-120">Relationships</span></span>
<span data-ttu-id="d1287-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d1287-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1287-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1287-122">JSON Representation</span></span>
<span data-ttu-id="d1287-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1287-123">Here is a JSON representation of the resource.</span></span>
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



