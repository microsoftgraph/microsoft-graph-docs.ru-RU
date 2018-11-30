---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
ms.openlocfilehash: 976191384afb563a8243b92dfa9ddfcc98f0c4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076923"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="f78a9-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f78a9-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="f78a9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f78a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f78a9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f78a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f78a9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f78a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f78a9-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="f78a9-107">The identifier for an Android app.</span></span>

<span data-ttu-id="f78a9-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="f78a9-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f78a9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f78a9-109">Properties</span></span>
|<span data-ttu-id="f78a9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f78a9-110">Property</span></span>|<span data-ttu-id="f78a9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f78a9-111">Type</span></span>|<span data-ttu-id="f78a9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f78a9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f78a9-113">packageId</span><span class="sxs-lookup"><span data-stu-id="f78a9-113">packageId</span></span>|<span data-ttu-id="f78a9-114">String</span><span class="sxs-lookup"><span data-stu-id="f78a9-114">String</span></span>|<span data-ttu-id="f78a9-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="f78a9-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f78a9-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f78a9-116">Relationships</span></span>
<span data-ttu-id="f78a9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f78a9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f78a9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f78a9-118">JSON Representation</span></span>
<span data-ttu-id="f78a9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f78a9-119">Here is a JSON representation of the resource.</span></span>
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





