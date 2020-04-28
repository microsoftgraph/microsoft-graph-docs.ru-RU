---
title: Тип ресурса Девицеманажементсеттингаппконстраинт
description: Ограничение, включающее параметр, содержит только доступные типы приложений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 012f20e69f79018ffecbac0ff4558687ec407bdd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443322"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="0eec0-103">Тип ресурса Девицеманажементсеттингаппконстраинт</span><span class="sxs-lookup"><span data-stu-id="0eec0-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="0eec0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eec0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0eec0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eec0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eec0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eec0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eec0-107">Ограничение, включающее параметр, содержит только доступные типы приложений.</span><span class="sxs-lookup"><span data-stu-id="0eec0-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="0eec0-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0eec0-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0eec0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0eec0-109">Properties</span></span>
|<span data-ttu-id="0eec0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eec0-110">Property</span></span>|<span data-ttu-id="0eec0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0eec0-111">Type</span></span>|<span data-ttu-id="0eec0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0eec0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eec0-113">суппортедтипес</span><span class="sxs-lookup"><span data-stu-id="0eec0-113">supportedTypes</span></span>|<span data-ttu-id="0eec0-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0eec0-114">String collection</span></span>|<span data-ttu-id="0eec0-115">Допустимые типы приложений, которые необходимо разрешить для этого параметра</span><span class="sxs-lookup"><span data-stu-id="0eec0-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="0eec0-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0eec0-116">Relationships</span></span>
<span data-ttu-id="0eec0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0eec0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eec0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0eec0-118">JSON Representation</span></span>
<span data-ttu-id="0eec0-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eec0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAppConstraint",
  "supportedTypes": [
    "String"
  ]
}
```



