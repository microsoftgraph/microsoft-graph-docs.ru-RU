---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 769f6a5172b7a84e9e75a2d7a8f701e195135823
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231026"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="20269-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="20269-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="20269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20269-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20269-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20269-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20269-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20269-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20269-107">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="20269-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="20269-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="20269-108">Properties</span></span>
|<span data-ttu-id="20269-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="20269-109">Property</span></span>|<span data-ttu-id="20269-110">Тип</span><span class="sxs-lookup"><span data-stu-id="20269-110">Type</span></span>|<span data-ttu-id="20269-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20269-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20269-112">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="20269-112">clientIdentifier</span></span>|<span data-ttu-id="20269-113">String</span><span class="sxs-lookup"><span data-stu-id="20269-113">String</span></span>|<span data-ttu-id="20269-114">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="20269-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="20269-115">Блокировка</span><span class="sxs-lookup"><span data-stu-id="20269-115">isBlocked</span></span>|<span data-ttu-id="20269-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="20269-116">Boolean</span></span>|<span data-ttu-id="20269-117">Состояние блокировки клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="20269-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="20269-118">Связи</span><span class="sxs-lookup"><span data-stu-id="20269-118">Relationships</span></span>
<span data-ttu-id="20269-119">Нет</span><span class="sxs-lookup"><span data-stu-id="20269-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20269-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20269-120">JSON Representation</span></span>
<span data-ttu-id="20269-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20269-121">Here is a JSON representation of the resource.</span></span>
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




