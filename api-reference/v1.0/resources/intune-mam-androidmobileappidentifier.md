---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc203cc9268849e8b7b46d994c166378252df59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871745"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="fd0b9-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd0b9-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="fd0b9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd0b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd0b9-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="fd0b9-105">The identifier for an Android app.</span></span>

<span data-ttu-id="fd0b9-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="fd0b9-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd0b9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd0b9-107">Properties</span></span>
|<span data-ttu-id="fd0b9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd0b9-108">Property</span></span>|<span data-ttu-id="fd0b9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fd0b9-109">Type</span></span>|<span data-ttu-id="fd0b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd0b9-111">packageId</span><span class="sxs-lookup"><span data-stu-id="fd0b9-111">packageId</span></span>|<span data-ttu-id="fd0b9-112">String</span><span class="sxs-lookup"><span data-stu-id="fd0b9-112">String</span></span>|<span data-ttu-id="fd0b9-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="fd0b9-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd0b9-114">Связи</span><span class="sxs-lookup"><span data-stu-id="fd0b9-114">Relationships</span></span>
<span data-ttu-id="fd0b9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="fd0b9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd0b9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd0b9-116">JSON Representation</span></span>
<span data-ttu-id="fd0b9-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd0b9-117">Here is a JSON representation of the resource.</span></span>
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



