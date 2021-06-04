---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b1dbebd30fecd15a916eef554bbdffd27b435f3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754527"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="48572-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="48572-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="48572-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48572-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48572-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="48572-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="48572-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="48572-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48572-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="48572-108">Properties</span></span>
|<span data-ttu-id="48572-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="48572-109">Property</span></span>|<span data-ttu-id="48572-110">Тип</span><span class="sxs-lookup"><span data-stu-id="48572-110">Type</span></span>|<span data-ttu-id="48572-111">Описание</span><span class="sxs-lookup"><span data-stu-id="48572-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48572-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="48572-112">bundleId</span></span>|<span data-ttu-id="48572-113">String</span><span class="sxs-lookup"><span data-stu-id="48572-113">String</span></span>|<span data-ttu-id="48572-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="48572-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48572-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="48572-115">Relationships</span></span>
<span data-ttu-id="48572-116">Нет</span><span class="sxs-lookup"><span data-stu-id="48572-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48572-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48572-117">JSON Representation</span></span>
<span data-ttu-id="48572-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48572-118">Here is a JSON representation of the resource.</span></span>
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




