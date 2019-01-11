---
title: Тип ресурса windowsKioskAzureADGroup
description: Класс, используемый для идентификации группу AzureAD для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16c2b17220a92f9f230b786238b1195e2af48d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849870"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="15725-103">Тип ресурса windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="15725-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="15725-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15725-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15725-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15725-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15725-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="15725-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15725-107">Класс, используемый для идентификации группу AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="15725-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="15725-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="15725-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15725-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="15725-109">Properties</span></span>
|<span data-ttu-id="15725-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="15725-110">Property</span></span>|<span data-ttu-id="15725-111">Тип</span><span class="sxs-lookup"><span data-stu-id="15725-111">Type</span></span>|<span data-ttu-id="15725-112">Описание</span><span class="sxs-lookup"><span data-stu-id="15725-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15725-113">displayName</span><span class="sxs-lookup"><span data-stu-id="15725-113">displayName</span></span>|<span data-ttu-id="15725-114">Строка</span><span class="sxs-lookup"><span data-stu-id="15725-114">String</span></span>|<span data-ttu-id="15725-115">Отображаемое имя группы AzureAD, будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="15725-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="15725-116">groupId</span><span class="sxs-lookup"><span data-stu-id="15725-116">groupId</span></span>|<span data-ttu-id="15725-117">Строка</span><span class="sxs-lookup"><span data-stu-id="15725-117">String</span></span>|<span data-ttu-id="15725-118">Идентификатор группы AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="15725-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="15725-119">Связи</span><span class="sxs-lookup"><span data-stu-id="15725-119">Relationships</span></span>
<span data-ttu-id="15725-120">Нет</span><span class="sxs-lookup"><span data-stu-id="15725-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15725-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15725-121">JSON Representation</span></span>
<span data-ttu-id="15725-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15725-122">Here is a JSON representation of the resource.</span></span>
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





