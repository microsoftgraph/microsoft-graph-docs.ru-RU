---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a45c31a7829102dfabee85f930be397dede17513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140105"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="2e4c8-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2e4c8-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="2e4c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e4c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e4c8-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-106">The identifier for an Android app.</span></span>


<span data-ttu-id="2e4c8-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="2e4c8-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e4c8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e4c8-108">Properties</span></span>
|<span data-ttu-id="2e4c8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e4c8-109">Property</span></span>|<span data-ttu-id="2e4c8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2e4c8-110">Type</span></span>|<span data-ttu-id="2e4c8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2e4c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e4c8-112">packageId</span><span class="sxs-lookup"><span data-stu-id="2e4c8-112">packageId</span></span>|<span data-ttu-id="2e4c8-113">String</span><span class="sxs-lookup"><span data-stu-id="2e4c8-113">String</span></span>|<span data-ttu-id="2e4c8-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e4c8-115">Связи</span><span class="sxs-lookup"><span data-stu-id="2e4c8-115">Relationships</span></span>
<span data-ttu-id="2e4c8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2e4c8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e4c8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e4c8-117">JSON Representation</span></span>
<span data-ttu-id="2e4c8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e4c8-118">Here is a JSON representation of the resource.</span></span>
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




