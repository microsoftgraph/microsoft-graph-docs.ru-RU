---
title: Тип ресурса deviceManagementExchangeAccessRule
description: Правила доступа устройств в Exchange.
ms.openlocfilehash: e59c81fdfe6cb6a0a7f7f952e6bfc8929bbc2633
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077774"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="f9e86-103">Тип ресурса deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="f9e86-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="f9e86-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9e86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9e86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9e86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9e86-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9e86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9e86-107">Правила доступа устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9e86-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="f9e86-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9e86-108">Properties</span></span>
|<span data-ttu-id="f9e86-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9e86-109">Property</span></span>|<span data-ttu-id="f9e86-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9e86-110">Type</span></span>|<span data-ttu-id="f9e86-111">Description</span><span class="sxs-lookup"><span data-stu-id="f9e86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e86-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="f9e86-112">deviceClass</span></span>|[<span data-ttu-id="f9e86-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="f9e86-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="f9e86-114">Класс устройства, который будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="f9e86-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f9e86-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f9e86-115">accessLevel</span></span>|[<span data-ttu-id="f9e86-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f9e86-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="f9e86-117">Уровень доступа для Exchange, предоставленных с этого правила.</span><span class="sxs-lookup"><span data-stu-id="f9e86-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="f9e86-118">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="f9e86-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9e86-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f9e86-119">Relationships</span></span>
<span data-ttu-id="f9e86-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f9e86-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9e86-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9e86-121">JSON Representation</span></span>
<span data-ttu-id="f9e86-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9e86-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```





