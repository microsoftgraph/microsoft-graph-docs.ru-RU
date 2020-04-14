---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e2930c95a62bb33d9beefb6501e89380da9b507
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469241"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="a8213-103">Тип ресурса Девицеманажементусерригхтссеттинг</span><span class="sxs-lookup"><span data-stu-id="a8213-103">deviceManagementUserRightsSetting resource type</span></span>

<span data-ttu-id="a8213-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8213-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8213-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8213-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8213-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8213-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8213-107">Представляет параметр прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8213-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="a8213-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8213-108">Properties</span></span>
|<span data-ttu-id="a8213-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8213-109">Property</span></span>|<span data-ttu-id="a8213-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8213-110">Type</span></span>|<span data-ttu-id="a8213-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8213-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8213-112">state</span><span class="sxs-lookup"><span data-stu-id="a8213-112">state</span></span>|[<span data-ttu-id="a8213-113">статеманажементсеттинг</span><span class="sxs-lookup"><span data-stu-id="a8213-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="a8213-114">Представляет текущее состояние этого параметра прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="a8213-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="a8213-115">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a8213-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="a8213-116">локалусерсорграупс</span><span class="sxs-lookup"><span data-stu-id="a8213-116">localUsersOrGroups</span></span>|<span data-ttu-id="a8213-117">Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a8213-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="a8213-118">Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено.</span><span class="sxs-lookup"><span data-stu-id="a8213-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="a8213-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8213-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8213-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="a8213-120">Relationships</span></span>
<span data-ttu-id="a8213-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a8213-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8213-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8213-122">JSON Representation</span></span>
<span data-ttu-id="a8213-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8213-123">Here is a JSON representation of the resource.</span></span>
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



