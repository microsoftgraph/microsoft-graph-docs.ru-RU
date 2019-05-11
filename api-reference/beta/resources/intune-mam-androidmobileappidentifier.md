---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ca2a2d9d548a94651514d1b3db2b385b5dc64bd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940906"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="c7049-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c7049-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c7049-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7049-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7049-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7049-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7049-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="c7049-106">The identifier for an Android app.</span></span>


<span data-ttu-id="c7049-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c7049-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7049-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7049-108">Properties</span></span>
|<span data-ttu-id="c7049-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7049-109">Property</span></span>|<span data-ttu-id="c7049-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c7049-110">Type</span></span>|<span data-ttu-id="c7049-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7049-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7049-112">packageId</span><span class="sxs-lookup"><span data-stu-id="c7049-112">packageId</span></span>|<span data-ttu-id="c7049-113">String</span><span class="sxs-lookup"><span data-stu-id="c7049-113">String</span></span>|<span data-ttu-id="c7049-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="c7049-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7049-115">Связи</span><span class="sxs-lookup"><span data-stu-id="c7049-115">Relationships</span></span>
<span data-ttu-id="c7049-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c7049-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7049-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7049-117">JSON Representation</span></span>
<span data-ttu-id="c7049-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7049-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




