---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
ms.openlocfilehash: 16f142c40083b9410f84e128951680ced269ea12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026826"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="b8f33-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8f33-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="b8f33-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8f33-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8f33-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="b8f33-105">The identifier for an Android app.</span></span>

<span data-ttu-id="b8f33-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="b8f33-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8f33-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8f33-107">Properties</span></span>
|<span data-ttu-id="b8f33-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8f33-108">Property</span></span>|<span data-ttu-id="b8f33-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8f33-109">Type</span></span>|<span data-ttu-id="b8f33-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8f33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8f33-111">packageId</span><span class="sxs-lookup"><span data-stu-id="b8f33-111">packageId</span></span>|<span data-ttu-id="b8f33-112">String</span><span class="sxs-lookup"><span data-stu-id="b8f33-112">String</span></span>|<span data-ttu-id="b8f33-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="b8f33-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8f33-114">Связи</span><span class="sxs-lookup"><span data-stu-id="b8f33-114">Relationships</span></span>
<span data-ttu-id="b8f33-115">Нет</span><span class="sxs-lookup"><span data-stu-id="b8f33-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8f33-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8f33-116">JSON Representation</span></span>
<span data-ttu-id="b8f33-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8f33-117">Here is a JSON representation of the resource.</span></span>
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



