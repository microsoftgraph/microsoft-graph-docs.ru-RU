---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd2ee1531c2bfe2399949d2e08a209826079cb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875840"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="4757c-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="4757c-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="4757c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4757c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4757c-105">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="4757c-105">The identifier for an iOS app.</span></span>

<span data-ttu-id="4757c-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="4757c-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4757c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4757c-107">Properties</span></span>
|<span data-ttu-id="4757c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4757c-108">Property</span></span>|<span data-ttu-id="4757c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4757c-109">Type</span></span>|<span data-ttu-id="4757c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4757c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4757c-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="4757c-111">bundleId</span></span>|<span data-ttu-id="4757c-112">String</span><span class="sxs-lookup"><span data-stu-id="4757c-112">String</span></span>|<span data-ttu-id="4757c-113">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="4757c-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4757c-114">Связи</span><span class="sxs-lookup"><span data-stu-id="4757c-114">Relationships</span></span>
<span data-ttu-id="4757c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="4757c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4757c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4757c-116">JSON Representation</span></span>
<span data-ttu-id="4757c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4757c-117">Here is a JSON representation of the resource.</span></span>
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



