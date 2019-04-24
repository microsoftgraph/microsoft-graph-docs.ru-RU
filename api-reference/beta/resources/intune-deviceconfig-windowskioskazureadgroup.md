---
title: Тип ресурса Виндовскиосказуреадграуп
description: Класс, используемый для идентификации группы AzureAD для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3224f55f4a5158fb8c0850a4dbea7e6bcf8d18d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522435"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="1b622-103">Тип ресурса Виндовскиосказуреадграуп</span><span class="sxs-lookup"><span data-stu-id="1b622-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="1b622-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b622-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b622-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b622-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b622-106">Класс, используемый для идентификации группы AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="1b622-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="1b622-107">НаСледуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="1b622-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b622-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b622-108">Properties</span></span>
|<span data-ttu-id="1b622-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b622-109">Property</span></span>|<span data-ttu-id="1b622-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1b622-110">Type</span></span>|<span data-ttu-id="1b622-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1b622-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b622-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1b622-112">displayName</span></span>|<span data-ttu-id="1b622-113">String</span><span class="sxs-lookup"><span data-stu-id="1b622-113">String</span></span>|<span data-ttu-id="1b622-114">Отображаемое имя группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="1b622-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="1b622-115">groupId</span><span class="sxs-lookup"><span data-stu-id="1b622-115">groupId</span></span>|<span data-ttu-id="1b622-116">String</span><span class="sxs-lookup"><span data-stu-id="1b622-116">String</span></span>|<span data-ttu-id="1b622-117">Идентификатор группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="1b622-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b622-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="1b622-118">Relationships</span></span>
<span data-ttu-id="1b622-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1b622-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b622-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b622-120">JSON Representation</span></span>
<span data-ttu-id="1b622-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b622-121">Here is a JSON representation of the resource.</span></span>
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





