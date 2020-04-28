---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 725847d0150a886ed11ce6d68cd49138711ede0f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465024"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="a9d95-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="a9d95-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="a9d95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9d95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9d95-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9d95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9d95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9d95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9d95-107">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="a9d95-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="a9d95-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9d95-108">Properties</span></span>
|<span data-ttu-id="a9d95-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9d95-109">Property</span></span>|<span data-ttu-id="a9d95-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a9d95-110">Type</span></span>|<span data-ttu-id="a9d95-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a9d95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9d95-112">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="a9d95-112">clientIdentifier</span></span>|<span data-ttu-id="a9d95-113">String</span><span class="sxs-lookup"><span data-stu-id="a9d95-113">String</span></span>|<span data-ttu-id="a9d95-114">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="a9d95-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="a9d95-115">Блокировка</span><span class="sxs-lookup"><span data-stu-id="a9d95-115">isBlocked</span></span>|<span data-ttu-id="a9d95-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d95-116">Boolean</span></span>|<span data-ttu-id="a9d95-117">Состояние блокировки клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="a9d95-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9d95-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a9d95-118">Relationships</span></span>
<span data-ttu-id="a9d95-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a9d95-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9d95-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9d95-120">JSON Representation</span></span>
<span data-ttu-id="a9d95-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9d95-121">Here is a JSON representation of the resource.</span></span>
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



