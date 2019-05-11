---
title: Тип ресурса Оффицеусерчеккинсуммари
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 9ee53bbdbb02a3d5716f49941ec108e23a09ae88
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949271"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="2e6cb-103">Тип ресурса Оффицеусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="2e6cb-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="2e6cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e6cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e6cb-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="2e6cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e6cb-107">Properties</span></span>
|<span data-ttu-id="2e6cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e6cb-108">Property</span></span>|<span data-ttu-id="2e6cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2e6cb-109">Type</span></span>|<span data-ttu-id="2e6cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e6cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e6cb-111">Сукцеедедусеркаунт</span><span class="sxs-lookup"><span data-stu-id="2e6cb-111">succeededUserCount</span></span>|<span data-ttu-id="2e6cb-112">Int32</span><span class="sxs-lookup"><span data-stu-id="2e6cb-112">Int32</span></span>|<span data-ttu-id="2e6cb-113">Общее количество успешных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="2e6cb-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="2e6cb-114">failedUserCount</span></span>|<span data-ttu-id="2e6cb-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2e6cb-115">Int32</span></span>|<span data-ttu-id="2e6cb-116">Общее число неудачных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e6cb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="2e6cb-117">Relationships</span></span>
<span data-ttu-id="2e6cb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="2e6cb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e6cb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e6cb-119">JSON Representation</span></span>
<span data-ttu-id="2e6cb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e6cb-120">Here is a JSON representation of the resource.</span></span>
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



