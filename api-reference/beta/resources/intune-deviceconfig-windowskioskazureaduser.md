---
title: Тип ресурса windowsKioskAzureADUser
description: Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420187"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="4f412-103">Тип ресурса windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="4f412-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="4f412-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f412-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f412-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f412-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f412-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f412-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f412-107">Класс, используемый для идентификации учетной записи пользователя в AzureAD для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="4f412-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="4f412-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4f412-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f412-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f412-109">Properties</span></span>
|<span data-ttu-id="4f412-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f412-110">Property</span></span>|<span data-ttu-id="4f412-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4f412-111">Type</span></span>|<span data-ttu-id="4f412-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4f412-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f412-113">userId</span><span class="sxs-lookup"><span data-stu-id="4f412-113">userId</span></span>|<span data-ttu-id="4f412-114">String</span><span class="sxs-lookup"><span data-stu-id="4f412-114">String</span></span>|<span data-ttu-id="4f412-115">Идентификатор пользователя AzureAD, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="4f412-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="4f412-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4f412-116">userPrincipalName</span></span>|<span data-ttu-id="4f412-117">String</span><span class="sxs-lookup"><span data-stu-id="4f412-117">String</span></span>|<span data-ttu-id="4f412-118">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="4f412-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f412-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f412-119">Relationships</span></span>
<span data-ttu-id="4f412-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4f412-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f412-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f412-121">JSON Representation</span></span>
<span data-ttu-id="4f412-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f412-122">Here is a JSON representation of the resource.</span></span>
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




