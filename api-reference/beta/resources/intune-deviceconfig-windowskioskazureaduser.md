---
title: Тип ресурса windowsKioskAzureADUser
description: Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57b48bcdbac3f95da37704222cded29ba61cd32d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845887"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="194ce-103">Тип ресурса windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="194ce-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="194ce-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="194ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="194ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="194ce-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="194ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="194ce-107">Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="194ce-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="194ce-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="194ce-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="194ce-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="194ce-109">Properties</span></span>
|<span data-ttu-id="194ce-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="194ce-110">Property</span></span>|<span data-ttu-id="194ce-111">Тип</span><span class="sxs-lookup"><span data-stu-id="194ce-111">Type</span></span>|<span data-ttu-id="194ce-112">Описание</span><span class="sxs-lookup"><span data-stu-id="194ce-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="194ce-113">userId</span><span class="sxs-lookup"><span data-stu-id="194ce-113">userId</span></span>|<span data-ttu-id="194ce-114">String</span><span class="sxs-lookup"><span data-stu-id="194ce-114">String</span></span>|<span data-ttu-id="194ce-115">Идентификатор пользователя AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="194ce-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="194ce-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="194ce-116">userPrincipalName</span></span>|<span data-ttu-id="194ce-117">Строка</span><span class="sxs-lookup"><span data-stu-id="194ce-117">String</span></span>|<span data-ttu-id="194ce-118">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="194ce-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="194ce-119">Связи</span><span class="sxs-lookup"><span data-stu-id="194ce-119">Relationships</span></span>
<span data-ttu-id="194ce-120">Нет</span><span class="sxs-lookup"><span data-stu-id="194ce-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="194ce-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="194ce-121">JSON Representation</span></span>
<span data-ttu-id="194ce-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="194ce-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





