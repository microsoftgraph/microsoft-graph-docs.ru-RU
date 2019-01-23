---
title: Тип ресурса deviceManagementUserRightsSetting
description: Представляет настройки прав пользователя.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35e6ec1a5faa5556a0e113df145d718c488b1669
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415056"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="0f594-103">Тип ресурса deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="0f594-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="0f594-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f594-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f594-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f594-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f594-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f594-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f594-107">Представляет настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f594-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="0f594-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f594-108">Properties</span></span>
|<span data-ttu-id="0f594-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f594-109">Property</span></span>|<span data-ttu-id="0f594-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f594-110">Type</span></span>|<span data-ttu-id="0f594-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f594-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f594-112">state</span><span class="sxs-lookup"><span data-stu-id="0f594-112">state</span></span>|[<span data-ttu-id="0f594-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="0f594-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="0f594-114">Представляющий текущее состояние этого пользователя права параметр.</span><span class="sxs-lookup"><span data-stu-id="0f594-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="0f594-115">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="0f594-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="0f594-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="0f594-116">localUsersOrGroups</span></span>|<span data-ttu-id="0f594-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0f594-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="0f594-118">Представляет коллекцию локальных пользователей или групп, которые установлены на устройстве, если состояние этого параметра разрешен.</span><span class="sxs-lookup"><span data-stu-id="0f594-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="0f594-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0f594-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f594-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0f594-120">Relationships</span></span>
<span data-ttu-id="0f594-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0f594-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f594-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f594-122">JSON Representation</span></span>
<span data-ttu-id="0f594-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f594-123">Here is a JSON representation of the resource.</span></span>
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




