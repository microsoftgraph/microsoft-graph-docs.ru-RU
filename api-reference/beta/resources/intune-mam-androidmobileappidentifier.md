---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c26c41ffcb36ee325f5e0fae907916a418fb8b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410282"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="9cf33-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9cf33-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="9cf33-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9cf33-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9cf33-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cf33-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cf33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf33-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="9cf33-107">The identifier for an Android app.</span></span>


<span data-ttu-id="9cf33-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="9cf33-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9cf33-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cf33-109">Properties</span></span>
|<span data-ttu-id="9cf33-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cf33-110">Property</span></span>|<span data-ttu-id="9cf33-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9cf33-111">Type</span></span>|<span data-ttu-id="9cf33-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9cf33-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf33-113">packageId</span><span class="sxs-lookup"><span data-stu-id="9cf33-113">packageId</span></span>|<span data-ttu-id="9cf33-114">String</span><span class="sxs-lookup"><span data-stu-id="9cf33-114">String</span></span>|<span data-ttu-id="9cf33-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="9cf33-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cf33-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9cf33-116">Relationships</span></span>
<span data-ttu-id="9cf33-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9cf33-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cf33-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cf33-118">JSON Representation</span></span>
<span data-ttu-id="9cf33-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cf33-119">Here is a JSON representation of the resource.</span></span>
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




