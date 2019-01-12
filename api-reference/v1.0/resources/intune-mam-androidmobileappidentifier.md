---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a940acc726467634df3a64dc686824350abf98f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915069"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="7f0e9-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f0e9-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="7f0e9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f0e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f0e9-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="7f0e9-105">The identifier for an Android app.</span></span>

<span data-ttu-id="7f0e9-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="7f0e9-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f0e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f0e9-107">Properties</span></span>
|<span data-ttu-id="7f0e9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f0e9-108">Property</span></span>|<span data-ttu-id="7f0e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f0e9-109">Type</span></span>|<span data-ttu-id="7f0e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f0e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f0e9-111">packageId</span><span class="sxs-lookup"><span data-stu-id="7f0e9-111">packageId</span></span>|<span data-ttu-id="7f0e9-112">String</span><span class="sxs-lookup"><span data-stu-id="7f0e9-112">String</span></span>|<span data-ttu-id="7f0e9-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="7f0e9-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f0e9-114">Связи</span><span class="sxs-lookup"><span data-stu-id="7f0e9-114">Relationships</span></span>
<span data-ttu-id="7f0e9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="7f0e9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f0e9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f0e9-116">JSON Representation</span></span>
<span data-ttu-id="7f0e9-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f0e9-117">Here is a JSON representation of the resource.</span></span>
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



