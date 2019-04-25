---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551850"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="67a63-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="67a63-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="67a63-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67a63-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a63-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="67a63-105">The identifier for an Android app.</span></span>


<span data-ttu-id="67a63-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="67a63-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67a63-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67a63-107">Properties</span></span>
|<span data-ttu-id="67a63-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="67a63-108">Property</span></span>|<span data-ttu-id="67a63-109">Тип</span><span class="sxs-lookup"><span data-stu-id="67a63-109">Type</span></span>|<span data-ttu-id="67a63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67a63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a63-111">packageId</span><span class="sxs-lookup"><span data-stu-id="67a63-111">packageId</span></span>|<span data-ttu-id="67a63-112">String</span><span class="sxs-lookup"><span data-stu-id="67a63-112">String</span></span>|<span data-ttu-id="67a63-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="67a63-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67a63-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="67a63-114">Relationships</span></span>
<span data-ttu-id="67a63-115">Нет</span><span class="sxs-lookup"><span data-stu-id="67a63-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67a63-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67a63-116">JSON Representation</span></span>
<span data-ttu-id="67a63-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67a63-117">Here is a JSON representation of the resource.</span></span>
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



