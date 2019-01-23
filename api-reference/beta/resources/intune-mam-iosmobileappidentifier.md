---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ddd09f6d1f0d49b00282c55bfa6dcbef1fcb1d2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409932"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="5085a-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5085a-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5085a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5085a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5085a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5085a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5085a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5085a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5085a-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="5085a-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="5085a-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5085a-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5085a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5085a-109">Properties</span></span>
|<span data-ttu-id="5085a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5085a-110">Property</span></span>|<span data-ttu-id="5085a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5085a-111">Type</span></span>|<span data-ttu-id="5085a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5085a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5085a-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="5085a-113">bundleId</span></span>|<span data-ttu-id="5085a-114">String</span><span class="sxs-lookup"><span data-stu-id="5085a-114">String</span></span>|<span data-ttu-id="5085a-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="5085a-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5085a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5085a-116">Relationships</span></span>
<span data-ttu-id="5085a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5085a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5085a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5085a-118">JSON Representation</span></span>
<span data-ttu-id="5085a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5085a-119">Here is a JSON representation of the resource.</span></span>
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




