---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2228e28b2edb3584a0861628644188d6fd54495b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802627"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="9aa92-103">Тип ресурса Девицеманажементусерригхтссеттинг</span><span class="sxs-lookup"><span data-stu-id="9aa92-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="9aa92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aa92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aa92-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9aa92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aa92-106">Представляет параметр прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="9aa92-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="9aa92-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9aa92-107">Properties</span></span>
|<span data-ttu-id="9aa92-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9aa92-108">Property</span></span>|<span data-ttu-id="9aa92-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9aa92-109">Type</span></span>|<span data-ttu-id="9aa92-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9aa92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa92-111">state</span><span class="sxs-lookup"><span data-stu-id="9aa92-111">state</span></span>|[<span data-ttu-id="9aa92-112">Статеманажементсеттинг</span><span class="sxs-lookup"><span data-stu-id="9aa92-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="9aa92-113">Представляет текущее состояние этого параметра прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="9aa92-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="9aa92-114">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="9aa92-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="9aa92-115">Локалусерсорграупс</span><span class="sxs-lookup"><span data-stu-id="9aa92-115">localUsersOrGroups</span></span>|<span data-ttu-id="9aa92-116">Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9aa92-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="9aa92-117">Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено.</span><span class="sxs-lookup"><span data-stu-id="9aa92-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="9aa92-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9aa92-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aa92-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="9aa92-119">Relationships</span></span>
<span data-ttu-id="9aa92-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9aa92-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aa92-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9aa92-121">JSON Representation</span></span>
<span data-ttu-id="9aa92-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9aa92-122">Here is a JSON representation of the resource.</span></span>
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





