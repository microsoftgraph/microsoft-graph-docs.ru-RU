---
title: Тип ресурса adminConsent
description: Сведения о разрешения администратора.
author: tfitzmac
ms.openlocfilehash: 7e535eb3475745c8c8aabb2701d9b9e24b8d3b02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354084"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="aa3b9-103">Тип ресурса adminConsent</span><span class="sxs-lookup"><span data-stu-id="aa3b9-103">adminConsent resource type</span></span>

> <span data-ttu-id="aa3b9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa3b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa3b9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa3b9-107">Сведения о разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="aa3b9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa3b9-108">Properties</span></span>
|<span data-ttu-id="aa3b9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa3b9-109">Property</span></span>|<span data-ttu-id="aa3b9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aa3b9-110">Type</span></span>|<span data-ttu-id="aa3b9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aa3b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa3b9-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="aa3b9-112">shareAPNSData</span></span>|[<span data-ttu-id="aa3b9-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="aa3b9-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="aa3b9-114">Состояние разрешения администратора общего доступа пользователей и данных устройства Apple.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="aa3b9-115">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa3b9-116">Связи</span><span class="sxs-lookup"><span data-stu-id="aa3b9-116">Relationships</span></span>
<span data-ttu-id="aa3b9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="aa3b9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa3b9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa3b9-118">JSON Representation</span></span>
<span data-ttu-id="aa3b9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa3b9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





