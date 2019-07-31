---
title: Тип ресурса Виндовскиосказуреадграуп
description: Класс, используемый для идентификации группы AzureAD для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2711b9e4adcb6cc0807b0fc16495909b1597623
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000314"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="5a1b7-103">Тип ресурса Виндовскиосказуреадграуп</span><span class="sxs-lookup"><span data-stu-id="5a1b7-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="5a1b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a1b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a1b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a1b7-106">Класс, используемый для идентификации группы AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="5a1b7-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="5a1b7-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="5a1b7-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a1b7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a1b7-108">Properties</span></span>
|<span data-ttu-id="5a1b7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a1b7-109">Property</span></span>|<span data-ttu-id="5a1b7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5a1b7-110">Type</span></span>|<span data-ttu-id="5a1b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5a1b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1b7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5a1b7-112">displayName</span></span>|<span data-ttu-id="5a1b7-113">String</span><span class="sxs-lookup"><span data-stu-id="5a1b7-113">String</span></span>|<span data-ttu-id="5a1b7-114">Отображаемое имя группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="5a1b7-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="5a1b7-115">groupId</span><span class="sxs-lookup"><span data-stu-id="5a1b7-115">groupId</span></span>|<span data-ttu-id="5a1b7-116">String</span><span class="sxs-lookup"><span data-stu-id="5a1b7-116">String</span></span>|<span data-ttu-id="5a1b7-117">Идентификатор группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="5a1b7-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a1b7-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a1b7-118">Relationships</span></span>
<span data-ttu-id="5a1b7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5a1b7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a1b7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a1b7-120">JSON Representation</span></span>
<span data-ttu-id="5a1b7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a1b7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





