---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a25dd46c8f1f8efdc3149472dae88910774e44a9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983374"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="751a1-103">Тип ресурса Adminconsent.</span><span class="sxs-lookup"><span data-stu-id="751a1-103">adminConsent resource type</span></span>

> <span data-ttu-id="751a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="751a1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="751a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751a1-106">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="751a1-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="751a1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="751a1-107">Properties</span></span>
|<span data-ttu-id="751a1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="751a1-108">Property</span></span>|<span data-ttu-id="751a1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="751a1-109">Type</span></span>|<span data-ttu-id="751a1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="751a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751a1-111">Шареапнсдата</span><span class="sxs-lookup"><span data-stu-id="751a1-111">shareAPNSData</span></span>|[<span data-ttu-id="751a1-112">Админконсентстате</span><span class="sxs-lookup"><span data-stu-id="751a1-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="751a1-113">Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple.</span><span class="sxs-lookup"><span data-stu-id="751a1-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="751a1-114">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="751a1-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="751a1-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="751a1-115">Relationships</span></span>
<span data-ttu-id="751a1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="751a1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="751a1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="751a1-117">JSON Representation</span></span>
<span data-ttu-id="751a1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="751a1-118">Here is a JSON representation of the resource.</span></span>
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





