---
title: Тип ресурса Девицеманажементусерригхтссеттинг
description: Представляет параметр прав пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fc278cab107533a1708bd116fc88bc0da947b608
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707810"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="08ddb-103">Тип ресурса Девицеманажементусерригхтссеттинг</span><span class="sxs-lookup"><span data-stu-id="08ddb-103">deviceManagementUserRightsSetting resource type</span></span>

<span data-ttu-id="08ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08ddb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08ddb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08ddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08ddb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08ddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ddb-107">Представляет параметр прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="08ddb-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="08ddb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="08ddb-108">Properties</span></span>
|<span data-ttu-id="08ddb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="08ddb-109">Property</span></span>|<span data-ttu-id="08ddb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="08ddb-110">Type</span></span>|<span data-ttu-id="08ddb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08ddb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08ddb-112">state</span><span class="sxs-lookup"><span data-stu-id="08ddb-112">state</span></span>|[<span data-ttu-id="08ddb-113">статеманажементсеттинг</span><span class="sxs-lookup"><span data-stu-id="08ddb-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="08ddb-114">Представляет текущее состояние этого параметра прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="08ddb-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="08ddb-115">Возможные значения: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="08ddb-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="08ddb-116">локалусерсорграупс</span><span class="sxs-lookup"><span data-stu-id="08ddb-116">localUsersOrGroups</span></span>|<span data-ttu-id="08ddb-117">Коллекция [девицеманажементусерригхтслокалусерорграуп](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="08ddb-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="08ddb-118">Представляет коллекцию локальных пользователей или групп, которые будут установлены на устройстве, если состояние этого параметра — разрешено.</span><span class="sxs-lookup"><span data-stu-id="08ddb-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="08ddb-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="08ddb-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08ddb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="08ddb-120">Relationships</span></span>
<span data-ttu-id="08ddb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="08ddb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08ddb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08ddb-122">JSON Representation</span></span>
<span data-ttu-id="08ddb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08ddb-123">Here is a JSON representation of the resource.</span></span>
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





