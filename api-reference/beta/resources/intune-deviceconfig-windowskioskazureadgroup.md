---
title: Тип ресурса windowsKioskAzureADGroup
description: Класс, используемый для идентификации группу AzureAD для базовой конфигурации
ms.openlocfilehash: 4853013c9c1e9d4c276ee5e2ba83cb8b36afd06c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075284"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="30cf5-103">Тип ресурса windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="30cf5-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="30cf5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30cf5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30cf5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30cf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30cf5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30cf5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30cf5-107">Класс, используемый для идентификации группу AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="30cf5-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="30cf5-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="30cf5-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30cf5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="30cf5-109">Properties</span></span>
|<span data-ttu-id="30cf5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="30cf5-110">Property</span></span>|<span data-ttu-id="30cf5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="30cf5-111">Type</span></span>|<span data-ttu-id="30cf5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="30cf5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cf5-113">displayName</span><span class="sxs-lookup"><span data-stu-id="30cf5-113">displayName</span></span>|<span data-ttu-id="30cf5-114">String</span><span class="sxs-lookup"><span data-stu-id="30cf5-114">String</span></span>|<span data-ttu-id="30cf5-115">Отображаемое имя группы AzureAD, будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="30cf5-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="30cf5-116">groupId</span><span class="sxs-lookup"><span data-stu-id="30cf5-116">groupId</span></span>|<span data-ttu-id="30cf5-117">String</span><span class="sxs-lookup"><span data-stu-id="30cf5-117">String</span></span>|<span data-ttu-id="30cf5-118">Идентификатор группы AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="30cf5-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="30cf5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="30cf5-119">Relationships</span></span>
<span data-ttu-id="30cf5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="30cf5-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30cf5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30cf5-121">JSON Representation</span></span>
<span data-ttu-id="30cf5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30cf5-122">Here is a JSON representation of the resource.</span></span>
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





