---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261175"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="15432-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="15432-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="15432-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15432-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15432-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="15432-105">The identifier for an Android app.</span></span>


<span data-ttu-id="15432-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="15432-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="15432-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15432-107">Properties</span></span>
|<span data-ttu-id="15432-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15432-108">Property</span></span>|<span data-ttu-id="15432-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15432-109">Type</span></span>|<span data-ttu-id="15432-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15432-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15432-111">packageId</span><span class="sxs-lookup"><span data-stu-id="15432-111">packageId</span></span>|<span data-ttu-id="15432-112">String</span><span class="sxs-lookup"><span data-stu-id="15432-112">String</span></span>|<span data-ttu-id="15432-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="15432-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15432-114">Связи</span><span class="sxs-lookup"><span data-stu-id="15432-114">Relationships</span></span>
<span data-ttu-id="15432-115">Нет</span><span class="sxs-lookup"><span data-stu-id="15432-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15432-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15432-116">JSON Representation</span></span>
<span data-ttu-id="15432-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15432-117">Here is a JSON representation of the resource.</span></span>
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



