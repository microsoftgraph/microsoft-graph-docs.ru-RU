---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b329d017aaf9f7d26d76f74198b2c5508e97ae2c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196982"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="23e73-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="23e73-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="23e73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23e73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23e73-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23e73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23e73-106">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="23e73-106">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="23e73-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="23e73-107">Properties</span></span>
|<span data-ttu-id="23e73-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="23e73-108">Property</span></span>|<span data-ttu-id="23e73-109">Тип</span><span class="sxs-lookup"><span data-stu-id="23e73-109">Type</span></span>|<span data-ttu-id="23e73-110">Описание</span><span class="sxs-lookup"><span data-stu-id="23e73-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23e73-111">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="23e73-111">clientIdentifier</span></span>|<span data-ttu-id="23e73-112">String.</span><span class="sxs-lookup"><span data-stu-id="23e73-112">String</span></span>|<span data-ttu-id="23e73-113">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="23e73-113">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="23e73-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="23e73-114">Relationships</span></span>
<span data-ttu-id="23e73-115">Нет</span><span class="sxs-lookup"><span data-stu-id="23e73-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23e73-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23e73-116">JSON Representation</span></span>
<span data-ttu-id="23e73-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23e73-117">Here is a JSON representation of the resource.</span></span>
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



