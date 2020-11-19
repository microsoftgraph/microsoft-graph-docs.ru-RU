---
title: Тип ресурса Виндовскиосказуреадграуп
description: Класс, используемый для идентификации группы AzureAD для конфигурации киоска
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1885128afdbac2c8603ac5ec400c66bde6be9471
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293553"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="eaacc-103">Тип ресурса Виндовскиосказуреадграуп</span><span class="sxs-lookup"><span data-stu-id="eaacc-103">windowsKioskAzureADGroup resource type</span></span>

<span data-ttu-id="eaacc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaacc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaacc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaacc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaacc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaacc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaacc-107">Класс, используемый для идентификации группы AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eaacc-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="eaacc-108">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="eaacc-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eaacc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaacc-109">Properties</span></span>
|<span data-ttu-id="eaacc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaacc-110">Property</span></span>|<span data-ttu-id="eaacc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eaacc-111">Type</span></span>|<span data-ttu-id="eaacc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eaacc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaacc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eaacc-113">displayName</span></span>|<span data-ttu-id="eaacc-114">String</span><span class="sxs-lookup"><span data-stu-id="eaacc-114">String</span></span>|<span data-ttu-id="eaacc-115">Отображаемое имя группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eaacc-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="eaacc-116">groupId</span><span class="sxs-lookup"><span data-stu-id="eaacc-116">groupId</span></span>|<span data-ttu-id="eaacc-117">String</span><span class="sxs-lookup"><span data-stu-id="eaacc-117">String</span></span>|<span data-ttu-id="eaacc-118">Идентификатор группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="eaacc-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaacc-119">Связи</span><span class="sxs-lookup"><span data-stu-id="eaacc-119">Relationships</span></span>
<span data-ttu-id="eaacc-120">Нет</span><span class="sxs-lookup"><span data-stu-id="eaacc-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaacc-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaacc-121">JSON Representation</span></span>
<span data-ttu-id="eaacc-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaacc-122">Here is a JSON representation of the resource.</span></span>
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




