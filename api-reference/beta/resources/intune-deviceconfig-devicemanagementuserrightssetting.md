---
title: Тип ресурса deviceManagementUserRightsSetting
description: Представляет настройки прав пользователя.
author: tfitzmac
ms.openlocfilehash: c58a1d3e9a352561a1abec87fa4efa90c599fd7a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313701"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="edae9-103">Тип ресурса deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="edae9-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="edae9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="edae9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edae9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edae9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="edae9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="edae9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edae9-107">Представляет настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="edae9-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="edae9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edae9-108">Properties</span></span>
|<span data-ttu-id="edae9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edae9-109">Property</span></span>|<span data-ttu-id="edae9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edae9-110">Type</span></span>|<span data-ttu-id="edae9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edae9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edae9-112">state</span><span class="sxs-lookup"><span data-stu-id="edae9-112">state</span></span>|[<span data-ttu-id="edae9-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="edae9-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="edae9-114">Представляющий текущее состояние этого пользователя права параметр.</span><span class="sxs-lookup"><span data-stu-id="edae9-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="edae9-115">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="edae9-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="edae9-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="edae9-116">localUsersOrGroups</span></span>|<span data-ttu-id="edae9-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="edae9-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="edae9-118">Представляет коллекцию локальных пользователей или групп, которые установлены на устройстве, если состояние этого параметра разрешен.</span><span class="sxs-lookup"><span data-stu-id="edae9-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="edae9-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="edae9-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edae9-120">Связи</span><span class="sxs-lookup"><span data-stu-id="edae9-120">Relationships</span></span>
<span data-ttu-id="edae9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="edae9-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="edae9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edae9-122">JSON Representation</span></span>
<span data-ttu-id="edae9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edae9-123">Here is a JSON representation of the resource.</span></span>
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





