---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44bd4e889ccf7311b9d7b2807000167f9612d89a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297989"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="aa350-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="aa350-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="aa350-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa350-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa350-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa350-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa350-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa350-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa350-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="aa350-107">The identifier for an Android app.</span></span>


<span data-ttu-id="aa350-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="aa350-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa350-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa350-109">Properties</span></span>
|<span data-ttu-id="aa350-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa350-110">Property</span></span>|<span data-ttu-id="aa350-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aa350-111">Type</span></span>|<span data-ttu-id="aa350-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aa350-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa350-113">packageId</span><span class="sxs-lookup"><span data-stu-id="aa350-113">packageId</span></span>|<span data-ttu-id="aa350-114">String</span><span class="sxs-lookup"><span data-stu-id="aa350-114">String</span></span>|<span data-ttu-id="aa350-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="aa350-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa350-116">Связи</span><span class="sxs-lookup"><span data-stu-id="aa350-116">Relationships</span></span>
<span data-ttu-id="aa350-117">Нет</span><span class="sxs-lookup"><span data-stu-id="aa350-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa350-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa350-118">JSON Representation</span></span>
<span data-ttu-id="aa350-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa350-119">Here is a JSON representation of the resource.</span></span>
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




