---
title: Тип ресурса Виндовскиосказуреадусер
description: Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96d91f585d8c762a2e1080d38bfd7cebb75e3acc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943951"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="10a28-103">Тип ресурса Виндовскиосказуреадусер</span><span class="sxs-lookup"><span data-stu-id="10a28-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="10a28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10a28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10a28-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10a28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10a28-106">Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="10a28-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="10a28-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="10a28-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10a28-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="10a28-108">Properties</span></span>
|<span data-ttu-id="10a28-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="10a28-109">Property</span></span>|<span data-ttu-id="10a28-110">Тип</span><span class="sxs-lookup"><span data-stu-id="10a28-110">Type</span></span>|<span data-ttu-id="10a28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10a28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a28-112">userId</span><span class="sxs-lookup"><span data-stu-id="10a28-112">userId</span></span>|<span data-ttu-id="10a28-113">String</span><span class="sxs-lookup"><span data-stu-id="10a28-113">String</span></span>|<span data-ttu-id="10a28-114">Идентификатор пользователя AzureAD, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="10a28-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="10a28-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10a28-115">userPrincipalName</span></span>|<span data-ttu-id="10a28-116">String</span><span class="sxs-lookup"><span data-stu-id="10a28-116">String</span></span>|<span data-ttu-id="10a28-117">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="10a28-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="10a28-118">Связи</span><span class="sxs-lookup"><span data-stu-id="10a28-118">Relationships</span></span>
<span data-ttu-id="10a28-119">Нет</span><span class="sxs-lookup"><span data-stu-id="10a28-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10a28-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10a28-120">JSON Representation</span></span>
<span data-ttu-id="10a28-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10a28-121">Here is a JSON representation of the resource.</span></span>
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




