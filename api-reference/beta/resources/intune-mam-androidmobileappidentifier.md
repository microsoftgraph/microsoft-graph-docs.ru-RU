---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cbdaa159a07378776b141e4465b29d4880477b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528000"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="df01a-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="df01a-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="df01a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="df01a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df01a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df01a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df01a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df01a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df01a-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="df01a-107">The identifier for an Android app.</span></span>


<span data-ttu-id="df01a-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="df01a-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df01a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="df01a-109">Properties</span></span>
|<span data-ttu-id="df01a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="df01a-110">Property</span></span>|<span data-ttu-id="df01a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="df01a-111">Type</span></span>|<span data-ttu-id="df01a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="df01a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df01a-113">packageId</span><span class="sxs-lookup"><span data-stu-id="df01a-113">packageId</span></span>|<span data-ttu-id="df01a-114">String</span><span class="sxs-lookup"><span data-stu-id="df01a-114">String</span></span>|<span data-ttu-id="df01a-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="df01a-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df01a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="df01a-116">Relationships</span></span>
<span data-ttu-id="df01a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="df01a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df01a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df01a-118">JSON Representation</span></span>
<span data-ttu-id="df01a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df01a-119">Here is a JSON representation of the resource.</span></span>
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



