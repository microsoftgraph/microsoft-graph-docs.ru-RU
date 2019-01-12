---
title: Тип ресурса windowsKioskAzureADGroup
description: Класс, используемый для идентификации группу AzureAD для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18ca386f0e1ee4647cff2a0ff5be9f2098d8f447
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964734"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="c3cf0-103">Тип ресурса windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="c3cf0-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="c3cf0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3cf0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3cf0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3cf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3cf0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c3cf0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3cf0-107">Класс, используемый для идентификации группу AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c3cf0-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="c3cf0-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c3cf0-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3cf0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3cf0-109">Properties</span></span>
|<span data-ttu-id="c3cf0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3cf0-110">Property</span></span>|<span data-ttu-id="c3cf0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c3cf0-111">Type</span></span>|<span data-ttu-id="c3cf0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c3cf0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3cf0-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c3cf0-113">displayName</span></span>|<span data-ttu-id="c3cf0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c3cf0-114">String</span></span>|<span data-ttu-id="c3cf0-115">Отображаемое имя группы AzureAD, будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c3cf0-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="c3cf0-116">groupId</span><span class="sxs-lookup"><span data-stu-id="c3cf0-116">groupId</span></span>|<span data-ttu-id="c3cf0-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c3cf0-117">String</span></span>|<span data-ttu-id="c3cf0-118">Идентификатор группы AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c3cf0-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3cf0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c3cf0-119">Relationships</span></span>
<span data-ttu-id="c3cf0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c3cf0-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3cf0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3cf0-121">JSON Representation</span></span>
<span data-ttu-id="c3cf0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3cf0-122">Here is a JSON representation of the resource.</span></span>
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





