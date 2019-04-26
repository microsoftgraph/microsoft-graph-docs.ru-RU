---
title: Тип ресурса Девицеманажементусерригхтслокалусерорграуп
description: Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdb49ef0b98e3d76d092b1ebf9574d6df8c47d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567202"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="ef4fb-103">Тип ресурса Девицеманажементусерригхтслокалусерорграуп</span><span class="sxs-lookup"><span data-stu-id="ef4fb-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="ef4fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef4fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef4fb-106">Представляет сведения для локального пользователя или группы, которые используются для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="ef4fb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef4fb-107">Properties</span></span>
|<span data-ttu-id="ef4fb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef4fb-108">Property</span></span>|<span data-ttu-id="ef4fb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ef4fb-109">Type</span></span>|<span data-ttu-id="ef4fb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef4fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef4fb-111">name</span><span class="sxs-lookup"><span data-stu-id="ef4fb-111">name</span></span>|<span data-ttu-id="ef4fb-112">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-112">String</span></span>|<span data-ttu-id="ef4fb-113">Имя локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="ef4fb-114">description</span><span class="sxs-lookup"><span data-stu-id="ef4fb-114">description</span></span>|<span data-ttu-id="ef4fb-115">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-115">String</span></span>|<span data-ttu-id="ef4fb-116">Описание локального пользователя или группы администратором.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="ef4fb-117">Секуритидентифиер</span><span class="sxs-lookup"><span data-stu-id="ef4fb-117">securityIdentifier</span></span>|<span data-ttu-id="ef4fb-118">String</span><span class="sxs-lookup"><span data-stu-id="ef4fb-118">String</span></span>|<span data-ttu-id="ef4fb-119">Идентификатор безопасности этого локального пользователя или группы (например, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="ef4fb-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef4fb-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="ef4fb-120">Relationships</span></span>
<span data-ttu-id="ef4fb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ef4fb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef4fb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef4fb-122">JSON Representation</span></span>
<span data-ttu-id="ef4fb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef4fb-123">Here is a JSON representation of the resource.</span></span>
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





