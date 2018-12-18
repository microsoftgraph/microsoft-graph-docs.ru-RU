---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
ms.openlocfilehash: fa55d84c3f676d23caeba1e5fda33166b60aaada
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350829"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="1f9b7-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f9b7-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1f9b7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f9b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f9b7-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="1f9b7-105">The identifier for an Android app.</span></span>

<span data-ttu-id="1f9b7-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1f9b7-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f9b7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f9b7-107">Properties</span></span>
|<span data-ttu-id="1f9b7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f9b7-108">Property</span></span>|<span data-ttu-id="1f9b7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f9b7-109">Type</span></span>|<span data-ttu-id="1f9b7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f9b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f9b7-111">packageId</span><span class="sxs-lookup"><span data-stu-id="1f9b7-111">packageId</span></span>|<span data-ttu-id="1f9b7-112">String</span><span class="sxs-lookup"><span data-stu-id="1f9b7-112">String</span></span>|<span data-ttu-id="1f9b7-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="1f9b7-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f9b7-114">Связи</span><span class="sxs-lookup"><span data-stu-id="1f9b7-114">Relationships</span></span>
<span data-ttu-id="1f9b7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1f9b7-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f9b7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f9b7-116">JSON Representation</span></span>
<span data-ttu-id="1f9b7-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f9b7-117">Here is a JSON representation of the resource.</span></span>
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



