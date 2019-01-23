---
title: Тип ресурса windowsKioskAzureADGroup
description: Класс, используемый для идентификации группу AzureAD для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392572"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="ca14b-103">Тип ресурса windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="ca14b-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="ca14b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca14b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca14b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca14b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca14b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca14b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca14b-107">Класс, используемый для идентификации группу AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="ca14b-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="ca14b-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ca14b-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca14b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca14b-109">Properties</span></span>
|<span data-ttu-id="ca14b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca14b-110">Property</span></span>|<span data-ttu-id="ca14b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ca14b-111">Type</span></span>|<span data-ttu-id="ca14b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ca14b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca14b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ca14b-113">displayName</span></span>|<span data-ttu-id="ca14b-114">String</span><span class="sxs-lookup"><span data-stu-id="ca14b-114">String</span></span>|<span data-ttu-id="ca14b-115">Отображаемое имя группы AzureAD, будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="ca14b-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="ca14b-116">groupId</span><span class="sxs-lookup"><span data-stu-id="ca14b-116">groupId</span></span>|<span data-ttu-id="ca14b-117">String</span><span class="sxs-lookup"><span data-stu-id="ca14b-117">String</span></span>|<span data-ttu-id="ca14b-118">Идентификатор группы AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="ca14b-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca14b-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="ca14b-119">Relationships</span></span>
<span data-ttu-id="ca14b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ca14b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca14b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca14b-121">JSON Representation</span></span>
<span data-ttu-id="ca14b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca14b-122">Here is a JSON representation of the resource.</span></span>
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




