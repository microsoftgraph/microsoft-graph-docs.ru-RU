---
title: тип ресурса officeUserCheckinSummary
description: Объект, описывая статистику регистрации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed81c3c152b0d81cfcdf15388fdc4db3a7612052
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759572"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="44ac6-103">тип ресурса officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="44ac6-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="44ac6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44ac6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44ac6-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ac6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ac6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44ac6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ac6-107">Объект, описывая статистику регистрации клиента.</span><span class="sxs-lookup"><span data-stu-id="44ac6-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="44ac6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44ac6-108">Properties</span></span>
|<span data-ttu-id="44ac6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ac6-109">Property</span></span>|<span data-ttu-id="44ac6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44ac6-110">Type</span></span>|<span data-ttu-id="44ac6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44ac6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ac6-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="44ac6-112">succeededUserCount</span></span>|<span data-ttu-id="44ac6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="44ac6-113">Int32</span></span>|<span data-ttu-id="44ac6-114">Общие успешные проверки пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="44ac6-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="44ac6-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="44ac6-115">failedUserCount</span></span>|<span data-ttu-id="44ac6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="44ac6-116">Int32</span></span>|<span data-ttu-id="44ac6-117">Итого неудавшейся проверки пользователей за последние 3 месяца.</span><span class="sxs-lookup"><span data-stu-id="44ac6-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44ac6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="44ac6-118">Relationships</span></span>
<span data-ttu-id="44ac6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="44ac6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44ac6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44ac6-120">JSON Representation</span></span>
<span data-ttu-id="44ac6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44ac6-121">Here is a JSON representation of the resource.</span></span>
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




