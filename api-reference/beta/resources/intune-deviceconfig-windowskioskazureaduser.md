---
title: Тип ресурса windowsKioskAzureADUser
description: Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации
ms.openlocfilehash: 22e71ab10ac7fb755050e8d6e5d19568bef2fae8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077993"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="4cc22-103">Тип ресурса windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="4cc22-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="4cc22-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4cc22-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cc22-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cc22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cc22-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cc22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cc22-107">Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="4cc22-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="4cc22-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4cc22-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cc22-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cc22-109">Properties</span></span>
|<span data-ttu-id="4cc22-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cc22-110">Property</span></span>|<span data-ttu-id="4cc22-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4cc22-111">Type</span></span>|<span data-ttu-id="4cc22-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4cc22-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cc22-113">userId</span><span class="sxs-lookup"><span data-stu-id="4cc22-113">userId</span></span>|<span data-ttu-id="4cc22-114">String</span><span class="sxs-lookup"><span data-stu-id="4cc22-114">String</span></span>|<span data-ttu-id="4cc22-115">Идентификатор пользователя AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="4cc22-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="4cc22-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4cc22-116">userPrincipalName</span></span>|<span data-ttu-id="4cc22-117">String</span><span class="sxs-lookup"><span data-stu-id="4cc22-117">String</span></span>|<span data-ttu-id="4cc22-118">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4cc22-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cc22-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4cc22-119">Relationships</span></span>
<span data-ttu-id="4cc22-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4cc22-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cc22-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cc22-121">JSON Representation</span></span>
<span data-ttu-id="4cc22-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cc22-122">Here is a JSON representation of the resource.</span></span>
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





