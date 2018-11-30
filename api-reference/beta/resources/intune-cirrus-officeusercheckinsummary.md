---
title: Тип ресурса officeUserCheckinSummary
description: Сущности, которая описывает клиента возврат stats.
ms.openlocfilehash: b8b3cc0c6129782a25a12cf22659cb6849a81e26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077228"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="c2f50-103">Тип ресурса officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c2f50-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="c2f50-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2f50-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2f50-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2f50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2f50-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2f50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2f50-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="c2f50-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c2f50-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2f50-108">Properties</span></span>
|<span data-ttu-id="c2f50-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2f50-109">Property</span></span>|<span data-ttu-id="c2f50-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2f50-110">Type</span></span>|<span data-ttu-id="c2f50-111">Description</span><span class="sxs-lookup"><span data-stu-id="c2f50-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f50-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="c2f50-112">succeededUserCount</span></span>|<span data-ttu-id="c2f50-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f50-113">Int32</span></span>|<span data-ttu-id="c2f50-114">Всего успешных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="c2f50-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="c2f50-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="c2f50-115">failedUserCount</span></span>|<span data-ttu-id="c2f50-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f50-116">Int32</span></span>|<span data-ttu-id="c2f50-117">Всего неудачных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="c2f50-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2f50-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c2f50-118">Relationships</span></span>
<span data-ttu-id="c2f50-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2f50-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2f50-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2f50-120">JSON Representation</span></span>
<span data-ttu-id="c2f50-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2f50-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



