---
title: Тип ресурса Оффицеусерчеккинсуммари
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8564f7d0d2fb06218b141b7e9369f2096bdec982
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462521"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="d3bc8-103">Тип ресурса Оффицеусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="d3bc8-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="d3bc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3bc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3bc8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3bc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3bc8-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="d3bc8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3bc8-108">Properties</span></span>
|<span data-ttu-id="d3bc8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3bc8-109">Property</span></span>|<span data-ttu-id="d3bc8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3bc8-110">Type</span></span>|<span data-ttu-id="d3bc8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3bc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3bc8-112">сукцеедедусеркаунт</span><span class="sxs-lookup"><span data-stu-id="d3bc8-112">succeededUserCount</span></span>|<span data-ttu-id="d3bc8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d3bc8-113">Int32</span></span>|<span data-ttu-id="d3bc8-114">Общее количество успешных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="d3bc8-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d3bc8-115">failedUserCount</span></span>|<span data-ttu-id="d3bc8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d3bc8-116">Int32</span></span>|<span data-ttu-id="d3bc8-117">Общее число неудачных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3bc8-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="d3bc8-118">Relationships</span></span>
<span data-ttu-id="d3bc8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d3bc8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3bc8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3bc8-120">JSON Representation</span></span>
<span data-ttu-id="d3bc8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3bc8-121">Here is a JSON representation of the resource.</span></span>
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



