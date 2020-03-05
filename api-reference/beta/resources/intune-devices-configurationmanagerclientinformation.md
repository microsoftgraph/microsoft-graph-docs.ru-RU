---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67c1a4b4a9ac570b4acd71a1ce819f9705fd32e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528674"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="da4be-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="da4be-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="da4be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da4be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da4be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da4be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da4be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da4be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da4be-107">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="da4be-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="da4be-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da4be-108">Properties</span></span>
|<span data-ttu-id="da4be-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da4be-109">Property</span></span>|<span data-ttu-id="da4be-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da4be-110">Type</span></span>|<span data-ttu-id="da4be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da4be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da4be-112">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="da4be-112">clientIdentifier</span></span>|<span data-ttu-id="da4be-113">String</span><span class="sxs-lookup"><span data-stu-id="da4be-113">String</span></span>|<span data-ttu-id="da4be-114">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="da4be-114">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="da4be-115">Связи</span><span class="sxs-lookup"><span data-stu-id="da4be-115">Relationships</span></span>
<span data-ttu-id="da4be-116">Нет</span><span class="sxs-lookup"><span data-stu-id="da4be-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da4be-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da4be-117">JSON Representation</span></span>
<span data-ttu-id="da4be-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da4be-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



