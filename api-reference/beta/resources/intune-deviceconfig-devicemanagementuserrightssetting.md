---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f17945232642df68e02a03ff0e1ec54ee5e220
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199371"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="cb996-103">Тип ресурса Девицеманажементусерригхтссеттинг</span><span class="sxs-lookup"><span data-stu-id="cb996-103">deviceManagementUserRightsSetting resource type</span></span>

<span data-ttu-id="cb996-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb996-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb996-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb996-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb996-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb996-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb996-107">Представляет параметр прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb996-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="cb996-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb996-108">Properties</span></span>
|<span data-ttu-id="cb996-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb996-109">Property</span></span>|<span data-ttu-id="cb996-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cb996-110">Type</span></span>|<span data-ttu-id="cb996-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb996-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb996-112">state</span><span class="sxs-lookup"><span data-stu-id="cb996-112">state</span></span>|[<span data-ttu-id="cb996-113">статеманажементсеттинг</span><span class="sxs-lookup"><span data-stu-id="cb996-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="cb996-114">Представляет текущее состояние этого параметра прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb996-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="cb996-115">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cb996-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="cb996-116">локалусерсорграупс</span><span class="sxs-lookup"><span data-stu-id="cb996-116">localUsersOrGroups</span></span>|<span data-ttu-id="cb996-117">Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cb996-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="cb996-118">Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено.</span><span class="sxs-lookup"><span data-stu-id="cb996-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="cb996-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cb996-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb996-120">Связи</span><span class="sxs-lookup"><span data-stu-id="cb996-120">Relationships</span></span>
<span data-ttu-id="cb996-121">Нет</span><span class="sxs-lookup"><span data-stu-id="cb996-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb996-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb996-122">JSON Representation</span></span>
<span data-ttu-id="cb996-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb996-123">Here is a JSON representation of the resource.</span></span>
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




