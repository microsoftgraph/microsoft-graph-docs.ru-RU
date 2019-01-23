---
title: Тип ресурса windowsKioskLocalUser
description: Класс, используемый для идентификации локальная учетная запись для базовой конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b808cdb6cb8bb8540a553104d2c00108341a3e14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392670"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="fa1ef-103">Тип ресурса windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="fa1ef-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="fa1ef-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa1ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa1ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa1ef-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa1ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa1ef-107">Класс, используемый для идентификации локальная учетная запись для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="fa1ef-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="fa1ef-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="fa1ef-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa1ef-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa1ef-109">Properties</span></span>
|<span data-ttu-id="fa1ef-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa1ef-110">Property</span></span>|<span data-ttu-id="fa1ef-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fa1ef-111">Type</span></span>|<span data-ttu-id="fa1ef-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fa1ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa1ef-113">userName</span><span class="sxs-lookup"><span data-stu-id="fa1ef-113">userName</span></span>|<span data-ttu-id="fa1ef-114">String</span><span class="sxs-lookup"><span data-stu-id="fa1ef-114">String</span></span>|<span data-ttu-id="fa1ef-115">Локальный пользователь, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="fa1ef-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa1ef-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="fa1ef-116">Relationships</span></span>
<span data-ttu-id="fa1ef-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fa1ef-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa1ef-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa1ef-118">JSON Representation</span></span>
<span data-ttu-id="fa1ef-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa1ef-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




