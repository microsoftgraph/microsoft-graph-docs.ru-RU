---
title: Тип ресурса iosStoreAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34a57d5aee554ddd47c0df863ff7fff373a7251a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408028"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="8a249-103">Тип ресурса iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="8a249-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8a249-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a249-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a249-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a249-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a249-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a249-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a249-107">Содержит свойства, используемые при назначении мобильного приложения из магазина iOS группе.</span><span class="sxs-lookup"><span data-stu-id="8a249-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="8a249-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8a249-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a249-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a249-109">Properties</span></span>
|<span data-ttu-id="8a249-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a249-110">Property</span></span>|<span data-ttu-id="8a249-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8a249-111">Type</span></span>|<span data-ttu-id="8a249-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8a249-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a249-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8a249-113">vpnConfigurationId</span></span>|<span data-ttu-id="8a249-114">String</span><span class="sxs-lookup"><span data-stu-id="8a249-114">String</span></span>|<span data-ttu-id="8a249-115">ИД конфигурации VPN, применяемой к этому приложению.</span><span class="sxs-lookup"><span data-stu-id="8a249-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a249-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8a249-116">Relationships</span></span>
<span data-ttu-id="8a249-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8a249-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a249-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a249-118">JSON Representation</span></span>
<span data-ttu-id="8a249-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a249-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```




