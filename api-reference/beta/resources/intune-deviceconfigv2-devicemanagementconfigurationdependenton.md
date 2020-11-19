---
title: Тип ресурса Девицеманажементконфигуратиондепендентон
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e4f4b542fa5d295a7abcd92665325b49349069
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242259"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a><span data-ttu-id="8ab06-103">Тип ресурса Девицеманажементконфигуратиондепендентон</span><span class="sxs-lookup"><span data-stu-id="8ab06-103">deviceManagementConfigurationDependentOn resource type</span></span>

<span data-ttu-id="8ab06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ab06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ab06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ab06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab06-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8ab06-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8ab06-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ab06-108">Properties</span></span>
|<span data-ttu-id="8ab06-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ab06-109">Property</span></span>|<span data-ttu-id="8ab06-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8ab06-110">Type</span></span>|<span data-ttu-id="8ab06-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab06-112">депендентон</span><span class="sxs-lookup"><span data-stu-id="8ab06-112">dependentOn</span></span>|<span data-ttu-id="8ab06-113">String</span><span class="sxs-lookup"><span data-stu-id="8ab06-113">String</span></span>|<span data-ttu-id="8ab06-114">Идентификатор параметра родительского или родительского параметров, зависящий от</span><span class="sxs-lookup"><span data-stu-id="8ab06-114">Identifier of parent setting/ parent setting option dependent on</span></span>|
|<span data-ttu-id="8ab06-115">парентсеттингид</span><span class="sxs-lookup"><span data-stu-id="8ab06-115">parentSettingId</span></span>|<span data-ttu-id="8ab06-116">String</span><span class="sxs-lookup"><span data-stu-id="8ab06-116">String</span></span>|<span data-ttu-id="8ab06-117">Идентификатор параметра parent или Parent ID, зависящий от</span><span class="sxs-lookup"><span data-stu-id="8ab06-117">Identifier of parent setting/ parent setting id dependent on</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab06-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8ab06-118">Relationships</span></span>
<span data-ttu-id="8ab06-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8ab06-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ab06-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ab06-120">JSON Representation</span></span>
<span data-ttu-id="8ab06-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ab06-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```




