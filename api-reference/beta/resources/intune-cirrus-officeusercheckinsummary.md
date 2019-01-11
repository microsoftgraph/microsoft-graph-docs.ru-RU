---
title: Тип ресурса officeUserCheckinSummary
description: Сущности, которая описывает клиента возврат stats.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2470b1e531f1b268d6797fe2692baf0031728b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834024"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="5b31b-103">Тип ресурса officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="5b31b-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="5b31b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b31b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b31b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b31b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b31b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5b31b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b31b-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="5b31b-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="5b31b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b31b-108">Properties</span></span>
|<span data-ttu-id="5b31b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b31b-109">Property</span></span>|<span data-ttu-id="5b31b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5b31b-110">Type</span></span>|<span data-ttu-id="5b31b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b31b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b31b-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="5b31b-112">succeededUserCount</span></span>|<span data-ttu-id="5b31b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5b31b-113">Int32</span></span>|<span data-ttu-id="5b31b-114">Всего успешных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="5b31b-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="5b31b-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5b31b-115">failedUserCount</span></span>|<span data-ttu-id="5b31b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5b31b-116">Int32</span></span>|<span data-ttu-id="5b31b-117">Всего неудачных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="5b31b-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b31b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="5b31b-118">Relationships</span></span>
<span data-ttu-id="5b31b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5b31b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b31b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b31b-120">JSON Representation</span></span>
<span data-ttu-id="5b31b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b31b-121">Here is a JSON representation of the resource.</span></span>
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



