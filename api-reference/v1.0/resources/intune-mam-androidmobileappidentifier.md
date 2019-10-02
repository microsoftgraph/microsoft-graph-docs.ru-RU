---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3d8e0c1df2b996a8ae13cbdd8ff3424f10a775a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356564"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="5c936-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5c936-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5c936-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c936-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c936-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="5c936-105">The identifier for an Android app.</span></span>


<span data-ttu-id="5c936-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5c936-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5c936-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c936-107">Properties</span></span>
|<span data-ttu-id="5c936-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c936-108">Property</span></span>|<span data-ttu-id="5c936-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5c936-109">Type</span></span>|<span data-ttu-id="5c936-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c936-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c936-111">packageId</span><span class="sxs-lookup"><span data-stu-id="5c936-111">packageId</span></span>|<span data-ttu-id="5c936-112">String</span><span class="sxs-lookup"><span data-stu-id="5c936-112">String</span></span>|<span data-ttu-id="5c936-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="5c936-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c936-114">Связи</span><span class="sxs-lookup"><span data-stu-id="5c936-114">Relationships</span></span>
<span data-ttu-id="5c936-115">Нет</span><span class="sxs-lookup"><span data-stu-id="5c936-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c936-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c936-116">JSON Representation</span></span>
<span data-ttu-id="5c936-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c936-117">Here is a JSON representation of the resource.</span></span>
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




