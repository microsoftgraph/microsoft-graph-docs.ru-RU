---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
ms.openlocfilehash: c8f590deb33faf1782e3e2ad38f0b65ab4f58eed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306883"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="11c0f-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="11c0f-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="11c0f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11c0f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11c0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11c0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11c0f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11c0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11c0f-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="11c0f-107">The identifier for an Android app.</span></span>

<span data-ttu-id="11c0f-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="11c0f-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11c0f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="11c0f-109">Properties</span></span>
|<span data-ttu-id="11c0f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="11c0f-110">Property</span></span>|<span data-ttu-id="11c0f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="11c0f-111">Type</span></span>|<span data-ttu-id="11c0f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="11c0f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c0f-113">packageId</span><span class="sxs-lookup"><span data-stu-id="11c0f-113">packageId</span></span>|<span data-ttu-id="11c0f-114">String</span><span class="sxs-lookup"><span data-stu-id="11c0f-114">String</span></span>|<span data-ttu-id="11c0f-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="11c0f-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11c0f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="11c0f-116">Relationships</span></span>
<span data-ttu-id="11c0f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="11c0f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11c0f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11c0f-118">JSON Representation</span></span>
<span data-ttu-id="11c0f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11c0f-119">Here is a JSON representation of the resource.</span></span>
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





