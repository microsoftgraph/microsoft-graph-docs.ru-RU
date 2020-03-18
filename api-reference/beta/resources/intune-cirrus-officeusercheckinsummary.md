---
title: Тип ресурса Оффицеусерчеккинсуммари
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef202194c8817e500d27a96ae3dbf4e5e1a8359
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797299"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="bace2-103">Тип ресурса Оффицеусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="bace2-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="bace2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bace2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bace2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bace2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bace2-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="bace2-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="bace2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bace2-107">Properties</span></span>
|<span data-ttu-id="bace2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bace2-108">Property</span></span>|<span data-ttu-id="bace2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bace2-109">Type</span></span>|<span data-ttu-id="bace2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bace2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bace2-111">сукцеедедусеркаунт</span><span class="sxs-lookup"><span data-stu-id="bace2-111">succeededUserCount</span></span>|<span data-ttu-id="bace2-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bace2-112">Int32</span></span>|<span data-ttu-id="bace2-113">Общее количество успешных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="bace2-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="bace2-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="bace2-114">failedUserCount</span></span>|<span data-ttu-id="bace2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="bace2-115">Int32</span></span>|<span data-ttu-id="bace2-116">Общее число неудачных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="bace2-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bace2-117">Связи</span><span class="sxs-lookup"><span data-stu-id="bace2-117">Relationships</span></span>
<span data-ttu-id="bace2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bace2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bace2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bace2-119">JSON Representation</span></span>
<span data-ttu-id="bace2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bace2-120">Here is a JSON representation of the resource.</span></span>
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



