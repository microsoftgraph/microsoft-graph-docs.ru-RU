---
title: Тип ресурса Конфигуратионманажерклиентинформатион
description: Данные клиента Configuration Manager, синхронизированные из SCCM
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae7d36b353b989d4256294872fba4c4f225d2668
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371564"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="ab0c0-103">Тип ресурса Конфигуратионманажерклиентинформатион</span><span class="sxs-lookup"><span data-stu-id="ab0c0-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="ab0c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab0c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab0c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab0c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab0c0-106">Данные клиента Configuration Manager, синхронизированные из SCCM</span><span class="sxs-lookup"><span data-stu-id="ab0c0-106">Configuration manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="ab0c0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab0c0-107">Properties</span></span>
|<span data-ttu-id="ab0c0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab0c0-108">Property</span></span>|<span data-ttu-id="ab0c0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ab0c0-109">Type</span></span>|<span data-ttu-id="ab0c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab0c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab0c0-111">клиентидентифиер</span><span class="sxs-lookup"><span data-stu-id="ab0c0-111">clientIdentifier</span></span>|<span data-ttu-id="ab0c0-112">String</span><span class="sxs-lookup"><span data-stu-id="ab0c0-112">String</span></span>|<span data-ttu-id="ab0c0-113">Идентификатор клиента Configuration Manager из SCCM</span><span class="sxs-lookup"><span data-stu-id="ab0c0-113">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab0c0-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab0c0-114">Relationships</span></span>
<span data-ttu-id="ab0c0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ab0c0-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab0c0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab0c0-116">JSON Representation</span></span>
<span data-ttu-id="ab0c0-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab0c0-117">Here is a JSON representation of the resource.</span></span>
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



