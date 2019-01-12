---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 134f6e27b6fb113516fd119211e245fd77b2ae75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919528"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="6b0a3-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="6b0a3-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="6b0a3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b0a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b0a3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b0a3-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="6b0a3-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="6b0a3-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6b0a3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b0a3-109">Properties</span></span>
|<span data-ttu-id="6b0a3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b0a3-110">Property</span></span>|<span data-ttu-id="6b0a3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6b0a3-111">Type</span></span>|<span data-ttu-id="6b0a3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6b0a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b0a3-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="6b0a3-113">bundleId</span></span>|<span data-ttu-id="6b0a3-114">String</span><span class="sxs-lookup"><span data-stu-id="6b0a3-114">String</span></span>|<span data-ttu-id="6b0a3-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b0a3-116">Связи</span><span class="sxs-lookup"><span data-stu-id="6b0a3-116">Relationships</span></span>
<span data-ttu-id="6b0a3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="6b0a3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b0a3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b0a3-118">JSON Representation</span></span>
<span data-ttu-id="6b0a3-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b0a3-119">Here is a JSON representation of the resource.</span></span>
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





