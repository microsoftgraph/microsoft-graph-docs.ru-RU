---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e844f54486e26a6e41fdb40b1fba2be08bac10fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488140"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="1a1fd-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="1a1fd-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="1a1fd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a1fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a1fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a1fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a1fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a1fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1fd-107">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="1a1fd-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="1a1fd-108">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1a1fd-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a1fd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a1fd-109">Properties</span></span>
|<span data-ttu-id="1a1fd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a1fd-110">Property</span></span>|<span data-ttu-id="1a1fd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1a1fd-111">Type</span></span>|<span data-ttu-id="1a1fd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1a1fd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1fd-113">groupId</span><span class="sxs-lookup"><span data-stu-id="1a1fd-113">groupId</span></span>|<span data-ttu-id="1a1fd-114">String</span><span class="sxs-lookup"><span data-stu-id="1a1fd-114">String</span></span>|<span data-ttu-id="1a1fd-115">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="1a1fd-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1fd-116">Связи</span><span class="sxs-lookup"><span data-stu-id="1a1fd-116">Relationships</span></span>
<span data-ttu-id="1a1fd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1a1fd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a1fd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a1fd-118">JSON Representation</span></span>
<span data-ttu-id="1a1fd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a1fd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



