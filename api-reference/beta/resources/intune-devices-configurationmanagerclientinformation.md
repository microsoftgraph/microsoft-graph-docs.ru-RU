---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b99db60922a93353cd1cc2cb6b85ff6b1241efe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690240"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="f2f9d-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="f2f9d-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="f2f9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2f9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2f9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f9d-107">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="f2f9d-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="f2f9d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2f9d-108">Properties</span></span>
|<span data-ttu-id="f2f9d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2f9d-109">Property</span></span>|<span data-ttu-id="f2f9d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f2f9d-110">Type</span></span>|<span data-ttu-id="f2f9d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f9d-112">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="f2f9d-112">clientIdentifier</span></span>|<span data-ttu-id="f2f9d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f2f9d-113">String</span></span>|<span data-ttu-id="f2f9d-114">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="f2f9d-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="f2f9d-115">Блокировка</span><span class="sxs-lookup"><span data-stu-id="f2f9d-115">isBlocked</span></span>|<span data-ttu-id="f2f9d-116">Логический</span><span class="sxs-lookup"><span data-stu-id="f2f9d-116">Boolean</span></span>|<span data-ttu-id="f2f9d-117">Состояние блокировки клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="f2f9d-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2f9d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f2f9d-118">Relationships</span></span>
<span data-ttu-id="f2f9d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f2f9d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2f9d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2f9d-120">JSON Representation</span></span>
<span data-ttu-id="f2f9d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2f9d-121">Here is a JSON representation of the resource.</span></span>
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





