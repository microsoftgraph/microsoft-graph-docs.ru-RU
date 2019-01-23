---
title: Тип ресурса officeUserCheckinSummary
description: Сущности, которая описывает клиента возврат stats.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411010"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="98bde-103">Тип ресурса officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="98bde-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="98bde-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98bde-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98bde-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98bde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98bde-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98bde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98bde-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="98bde-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="98bde-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98bde-108">Properties</span></span>
|<span data-ttu-id="98bde-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98bde-109">Property</span></span>|<span data-ttu-id="98bde-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98bde-110">Type</span></span>|<span data-ttu-id="98bde-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98bde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98bde-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="98bde-112">succeededUserCount</span></span>|<span data-ttu-id="98bde-113">Int32</span><span class="sxs-lookup"><span data-stu-id="98bde-113">Int32</span></span>|<span data-ttu-id="98bde-114">Всего успешных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="98bde-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="98bde-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="98bde-115">failedUserCount</span></span>|<span data-ttu-id="98bde-116">Int32</span><span class="sxs-lookup"><span data-stu-id="98bde-116">Int32</span></span>|<span data-ttu-id="98bde-117">Всего неудачных пользователя проверьте ins за последние три месяца.</span><span class="sxs-lookup"><span data-stu-id="98bde-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98bde-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="98bde-118">Relationships</span></span>
<span data-ttu-id="98bde-119">Нет</span><span class="sxs-lookup"><span data-stu-id="98bde-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98bde-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98bde-120">JSON Representation</span></span>
<span data-ttu-id="98bde-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98bde-121">Here is a JSON representation of the resource.</span></span>
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



