---
title: Тип ресурса officeUserCheckinSummary
description: Сущности, которая описывает клиента возврат stats.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 374f5113a517b52ae7af6381f575ac60e5d00ae4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946583"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="ebd6f-103">Тип ресурса officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="ebd6f-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="ebd6f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebd6f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebd6f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebd6f-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="ebd6f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebd6f-108">Properties</span></span>
|<span data-ttu-id="ebd6f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebd6f-109">Property</span></span>|<span data-ttu-id="ebd6f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ebd6f-110">Type</span></span>|<span data-ttu-id="ebd6f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ebd6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd6f-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="ebd6f-112">succeededUserCount</span></span>|<span data-ttu-id="ebd6f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd6f-113">Int32</span></span>|<span data-ttu-id="ebd6f-114">Всего успешных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="ebd6f-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ebd6f-115">failedUserCount</span></span>|<span data-ttu-id="ebd6f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd6f-116">Int32</span></span>|<span data-ttu-id="ebd6f-117">Всего неудачных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd6f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ebd6f-118">Relationships</span></span>
<span data-ttu-id="ebd6f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ebd6f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ebd6f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebd6f-120">JSON Representation</span></span>
<span data-ttu-id="ebd6f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebd6f-121">Here is a JSON representation of the resource.</span></span>
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



