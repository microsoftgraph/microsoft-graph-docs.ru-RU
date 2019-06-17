---
title: Тип ресурса Виндовскиосказуреадусер
description: Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa938ff2b99f583255c18111f24b5e5f4d7a17b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978530"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="7e778-103">Тип ресурса Виндовскиосказуреадусер</span><span class="sxs-lookup"><span data-stu-id="7e778-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="7e778-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e778-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e778-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e778-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e778-106">Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="7e778-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="7e778-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="7e778-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e778-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e778-108">Properties</span></span>
|<span data-ttu-id="7e778-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e778-109">Property</span></span>|<span data-ttu-id="7e778-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7e778-110">Type</span></span>|<span data-ttu-id="7e778-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7e778-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e778-112">userId</span><span class="sxs-lookup"><span data-stu-id="7e778-112">userId</span></span>|<span data-ttu-id="7e778-113">String</span><span class="sxs-lookup"><span data-stu-id="7e778-113">String</span></span>|<span data-ttu-id="7e778-114">Идентификатор пользователя AzureAD, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="7e778-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="7e778-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e778-115">userPrincipalName</span></span>|<span data-ttu-id="7e778-116">String</span><span class="sxs-lookup"><span data-stu-id="7e778-116">String</span></span>|<span data-ttu-id="7e778-117">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="7e778-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e778-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="7e778-118">Relationships</span></span>
<span data-ttu-id="7e778-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7e778-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e778-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e778-120">JSON Representation</span></span>
<span data-ttu-id="7e778-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e778-121">Here is a JSON representation of the resource.</span></span>
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





