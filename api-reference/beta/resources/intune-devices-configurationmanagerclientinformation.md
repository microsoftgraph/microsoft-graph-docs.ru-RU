---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c9e9b88677c925fb33c998af571b23090dcff5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785058"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="b9d8d-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="b9d8d-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="b9d8d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9d8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9d8d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9d8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9d8d-106">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="b9d8d-106">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="b9d8d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9d8d-107">Properties</span></span>
|<span data-ttu-id="b9d8d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9d8d-108">Property</span></span>|<span data-ttu-id="b9d8d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9d8d-109">Type</span></span>|<span data-ttu-id="b9d8d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9d8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d8d-111">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="b9d8d-111">clientIdentifier</span></span>|<span data-ttu-id="b9d8d-112">String</span><span class="sxs-lookup"><span data-stu-id="b9d8d-112">String</span></span>|<span data-ttu-id="b9d8d-113">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="b9d8d-113">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="b9d8d-114">Блокировка</span><span class="sxs-lookup"><span data-stu-id="b9d8d-114">isBlocked</span></span>|<span data-ttu-id="b9d8d-115">Логический</span><span class="sxs-lookup"><span data-stu-id="b9d8d-115">Boolean</span></span>|<span data-ttu-id="b9d8d-116">Состояние блокировки клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="b9d8d-116">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9d8d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b9d8d-117">Relationships</span></span>
<span data-ttu-id="b9d8d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b9d8d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9d8d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9d8d-119">JSON Representation</span></span>
<span data-ttu-id="b9d8d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9d8d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```



