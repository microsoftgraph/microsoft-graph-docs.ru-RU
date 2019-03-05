---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f46e379a47bd7b08be1427115c785452543dfbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157941"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="a6b26-103">Тип ресурса Adminconsent.</span><span class="sxs-lookup"><span data-stu-id="a6b26-103">adminConsent resource type</span></span>

> <span data-ttu-id="a6b26-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6b26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6b26-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6b26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6b26-106">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="a6b26-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="a6b26-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6b26-107">Properties</span></span>
|<span data-ttu-id="a6b26-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6b26-108">Property</span></span>|<span data-ttu-id="a6b26-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a6b26-109">Type</span></span>|<span data-ttu-id="a6b26-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6b26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b26-111">Шареапнсдата</span><span class="sxs-lookup"><span data-stu-id="a6b26-111">shareAPNSData</span></span>|[<span data-ttu-id="a6b26-112">Админконсентстате</span><span class="sxs-lookup"><span data-stu-id="a6b26-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="a6b26-113">Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple.</span><span class="sxs-lookup"><span data-stu-id="a6b26-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="a6b26-114">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="a6b26-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6b26-115">Связи</span><span class="sxs-lookup"><span data-stu-id="a6b26-115">Relationships</span></span>
<span data-ttu-id="a6b26-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a6b26-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6b26-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6b26-117">JSON Representation</span></span>
<span data-ttu-id="a6b26-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6b26-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




