---
title: Тип ресурса Виндовскиосказуреадусер
description: Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 950d1bfeaf73f2f3a37cbd7c154323baf603aebd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786413"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="c2d4e-103">Тип ресурса Виндовскиосказуреадусер</span><span class="sxs-lookup"><span data-stu-id="c2d4e-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="c2d4e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2d4e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2d4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2d4e-106">Класс, используемый для определения учетной записи пользователя AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c2d4e-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="c2d4e-107">Наследуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c2d4e-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2d4e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d4e-108">Properties</span></span>
|<span data-ttu-id="c2d4e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d4e-109">Property</span></span>|<span data-ttu-id="c2d4e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d4e-110">Type</span></span>|<span data-ttu-id="c2d4e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d4e-112">userId</span><span class="sxs-lookup"><span data-stu-id="c2d4e-112">userId</span></span>|<span data-ttu-id="c2d4e-113">String</span><span class="sxs-lookup"><span data-stu-id="c2d4e-113">String</span></span>|<span data-ttu-id="c2d4e-114">Идентификатор пользователя AzureAD, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c2d4e-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="c2d4e-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2d4e-115">userPrincipalName</span></span>|<span data-ttu-id="c2d4e-116">String</span><span class="sxs-lookup"><span data-stu-id="c2d4e-116">String</span></span>|<span data-ttu-id="c2d4e-117">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c2d4e-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2d4e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c2d4e-118">Relationships</span></span>
<span data-ttu-id="c2d4e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2d4e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2d4e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d4e-120">JSON Representation</span></span>
<span data-ttu-id="c2d4e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d4e-121">Here is a JSON representation of the resource.</span></span>
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



