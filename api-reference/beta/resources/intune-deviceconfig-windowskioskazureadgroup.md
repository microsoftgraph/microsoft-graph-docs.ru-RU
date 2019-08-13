---
title: Тип ресурса Виндовскиосказуреадграуп
description: Класс, используемый для идентификации группы AzureAD для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00cd2f43fb09df03dfe2f5ee1810871dc2b77fb2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370944"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="35c88-103">Тип ресурса Виндовскиосказуреадграуп</span><span class="sxs-lookup"><span data-stu-id="35c88-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="35c88-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35c88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35c88-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35c88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35c88-106">Класс, используемый для идентификации группы AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="35c88-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="35c88-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="35c88-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35c88-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35c88-108">Properties</span></span>
|<span data-ttu-id="35c88-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35c88-109">Property</span></span>|<span data-ttu-id="35c88-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35c88-110">Type</span></span>|<span data-ttu-id="35c88-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35c88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c88-112">displayName</span><span class="sxs-lookup"><span data-stu-id="35c88-112">displayName</span></span>|<span data-ttu-id="35c88-113">String</span><span class="sxs-lookup"><span data-stu-id="35c88-113">String</span></span>|<span data-ttu-id="35c88-114">Отображаемое имя группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="35c88-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="35c88-115">groupId</span><span class="sxs-lookup"><span data-stu-id="35c88-115">groupId</span></span>|<span data-ttu-id="35c88-116">String</span><span class="sxs-lookup"><span data-stu-id="35c88-116">String</span></span>|<span data-ttu-id="35c88-117">Идентификатор группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="35c88-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="35c88-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="35c88-118">Relationships</span></span>
<span data-ttu-id="35c88-119">Нет</span><span class="sxs-lookup"><span data-stu-id="35c88-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c88-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35c88-120">JSON Representation</span></span>
<span data-ttu-id="35c88-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35c88-121">Here is a JSON representation of the resource.</span></span>
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



