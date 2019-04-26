---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2228e28b2edb3584a0861628644188d6fd54495b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567223"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="869a6-103">Тип ресурса Девицеманажементусерригхтссеттинг</span><span class="sxs-lookup"><span data-stu-id="869a6-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="869a6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="869a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="869a6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="869a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869a6-106">Представляет параметр прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="869a6-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="869a6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="869a6-107">Properties</span></span>
|<span data-ttu-id="869a6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="869a6-108">Property</span></span>|<span data-ttu-id="869a6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="869a6-109">Type</span></span>|<span data-ttu-id="869a6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="869a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="869a6-111">state</span><span class="sxs-lookup"><span data-stu-id="869a6-111">state</span></span>|[<span data-ttu-id="869a6-112">Статеманажементсеттинг</span><span class="sxs-lookup"><span data-stu-id="869a6-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="869a6-113">Представляет текущее состояние этого параметра прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="869a6-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="869a6-114">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="869a6-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="869a6-115">Локалусерсорграупс</span><span class="sxs-lookup"><span data-stu-id="869a6-115">localUsersOrGroups</span></span>|<span data-ttu-id="869a6-116">Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="869a6-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="869a6-117">Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено.</span><span class="sxs-lookup"><span data-stu-id="869a6-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="869a6-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="869a6-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="869a6-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="869a6-119">Relationships</span></span>
<span data-ttu-id="869a6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="869a6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="869a6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="869a6-121">JSON Representation</span></span>
<span data-ttu-id="869a6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="869a6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```





