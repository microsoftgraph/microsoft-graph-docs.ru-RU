---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07dcc1bd7480439f5c1dd71afa36e18a5df0eb14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754534"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="afded-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="afded-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="afded-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afded-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afded-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="afded-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afded-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="afded-106">The identifier for an Android app.</span></span>


<span data-ttu-id="afded-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="afded-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afded-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="afded-108">Properties</span></span>
|<span data-ttu-id="afded-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="afded-109">Property</span></span>|<span data-ttu-id="afded-110">Тип</span><span class="sxs-lookup"><span data-stu-id="afded-110">Type</span></span>|<span data-ttu-id="afded-111">Описание</span><span class="sxs-lookup"><span data-stu-id="afded-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afded-112">packageId</span><span class="sxs-lookup"><span data-stu-id="afded-112">packageId</span></span>|<span data-ttu-id="afded-113">String</span><span class="sxs-lookup"><span data-stu-id="afded-113">String</span></span>|<span data-ttu-id="afded-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="afded-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afded-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="afded-115">Relationships</span></span>
<span data-ttu-id="afded-116">Нет</span><span class="sxs-lookup"><span data-stu-id="afded-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afded-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afded-117">JSON Representation</span></span>
<span data-ttu-id="afded-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afded-118">Here is a JSON representation of the resource.</span></span>
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




