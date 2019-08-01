---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7388e6872eb48d3aba188448c263f492d913f79b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038152"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="fdb40-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fdb40-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="fdb40-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdb40-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdb40-105">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="fdb40-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="fdb40-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="fdb40-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdb40-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdb40-107">Properties</span></span>
|<span data-ttu-id="fdb40-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdb40-108">Property</span></span>|<span data-ttu-id="fdb40-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fdb40-109">Type</span></span>|<span data-ttu-id="fdb40-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fdb40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb40-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="fdb40-111">bundleId</span></span>|<span data-ttu-id="fdb40-112">String</span><span class="sxs-lookup"><span data-stu-id="fdb40-112">String</span></span>|<span data-ttu-id="fdb40-113">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="fdb40-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb40-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="fdb40-114">Relationships</span></span>
<span data-ttu-id="fdb40-115">Нет</span><span class="sxs-lookup"><span data-stu-id="fdb40-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdb40-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdb40-116">JSON Representation</span></span>
<span data-ttu-id="fdb40-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdb40-117">Here is a JSON representation of the resource.</span></span>
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



