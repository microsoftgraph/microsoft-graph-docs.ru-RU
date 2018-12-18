---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
ms.openlocfilehash: e68bfcca4b0873013c0c9e0fd0295483257ae52c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354175"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="2ad01-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ad01-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="2ad01-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2ad01-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ad01-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ad01-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ad01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ad01-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="2ad01-107">The identifier for an iOS app.</span></span>

<span data-ttu-id="2ad01-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="2ad01-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ad01-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ad01-109">Properties</span></span>
|<span data-ttu-id="2ad01-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ad01-110">Property</span></span>|<span data-ttu-id="2ad01-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad01-111">Type</span></span>|<span data-ttu-id="2ad01-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad01-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad01-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="2ad01-113">bundleId</span></span>|<span data-ttu-id="2ad01-114">String</span><span class="sxs-lookup"><span data-stu-id="2ad01-114">String</span></span>|<span data-ttu-id="2ad01-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="2ad01-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ad01-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2ad01-116">Relationships</span></span>
<span data-ttu-id="2ad01-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2ad01-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ad01-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ad01-118">JSON Representation</span></span>
<span data-ttu-id="2ad01-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ad01-119">Here is a JSON representation of the resource.</span></span>
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





