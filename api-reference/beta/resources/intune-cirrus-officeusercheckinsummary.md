---
title: Тип ресурса Оффицеусерчеккинсуммари
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a5719bef78f4a9c474f2ea896c6bd5d43de8f6d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723957"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="1cc1f-103">Тип ресурса Оффицеусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="1cc1f-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="1cc1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cc1f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cc1f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cc1f-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="1cc1f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cc1f-108">Properties</span></span>
|<span data-ttu-id="1cc1f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cc1f-109">Property</span></span>|<span data-ttu-id="1cc1f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1cc1f-110">Type</span></span>|<span data-ttu-id="1cc1f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1cc1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cc1f-112">сукцеедедусеркаунт</span><span class="sxs-lookup"><span data-stu-id="1cc1f-112">succeededUserCount</span></span>|<span data-ttu-id="1cc1f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1cc1f-113">Int32</span></span>|<span data-ttu-id="1cc1f-114">Общее количество успешных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="1cc1f-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="1cc1f-115">failedUserCount</span></span>|<span data-ttu-id="1cc1f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1cc1f-116">Int32</span></span>|<span data-ttu-id="1cc1f-117">Общее число неудачных проверок пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc1f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1cc1f-118">Relationships</span></span>
<span data-ttu-id="1cc1f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1cc1f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc1f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cc1f-120">JSON Representation</span></span>
<span data-ttu-id="1cc1f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-121">Here is a JSON representation of the resource.</span></span>
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





