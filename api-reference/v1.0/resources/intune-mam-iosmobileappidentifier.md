---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0eaade90c88cc553072f30dd36c42db4f44513
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249965"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="a420d-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a420d-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="a420d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a420d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a420d-105">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="a420d-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="a420d-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="a420d-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a420d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a420d-107">Properties</span></span>
|<span data-ttu-id="a420d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a420d-108">Property</span></span>|<span data-ttu-id="a420d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a420d-109">Type</span></span>|<span data-ttu-id="a420d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a420d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a420d-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="a420d-111">bundleId</span></span>|<span data-ttu-id="a420d-112">String</span><span class="sxs-lookup"><span data-stu-id="a420d-112">String</span></span>|<span data-ttu-id="a420d-113">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="a420d-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a420d-114">Связи</span><span class="sxs-lookup"><span data-stu-id="a420d-114">Relationships</span></span>
<span data-ttu-id="a420d-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a420d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a420d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a420d-116">JSON Representation</span></span>
<span data-ttu-id="a420d-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a420d-117">Here is a JSON representation of the resource.</span></span>
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



