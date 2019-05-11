---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7da88947c4033f1af615f85267a23426c5e4154
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940878"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="5946f-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5946f-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5946f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5946f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5946f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5946f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5946f-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="5946f-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="5946f-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5946f-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5946f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5946f-108">Properties</span></span>
|<span data-ttu-id="5946f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5946f-109">Property</span></span>|<span data-ttu-id="5946f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5946f-110">Type</span></span>|<span data-ttu-id="5946f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5946f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5946f-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="5946f-112">bundleId</span></span>|<span data-ttu-id="5946f-113">String</span><span class="sxs-lookup"><span data-stu-id="5946f-113">String</span></span>|<span data-ttu-id="5946f-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="5946f-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5946f-115">Связи</span><span class="sxs-lookup"><span data-stu-id="5946f-115">Relationships</span></span>
<span data-ttu-id="5946f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5946f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5946f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5946f-117">JSON Representation</span></span>
<span data-ttu-id="5946f-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5946f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




