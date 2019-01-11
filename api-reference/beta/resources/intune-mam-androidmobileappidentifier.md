---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 59c947192cf00e1f6852c51513692123595c975b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837594"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="5cb05-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5cb05-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="5cb05-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cb05-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cb05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cb05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cb05-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5cb05-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cb05-107">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="5cb05-107">The identifier for an Android app.</span></span>

<span data-ttu-id="5cb05-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="5cb05-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5cb05-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cb05-109">Properties</span></span>
|<span data-ttu-id="5cb05-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cb05-110">Property</span></span>|<span data-ttu-id="5cb05-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5cb05-111">Type</span></span>|<span data-ttu-id="5cb05-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5cb05-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cb05-113">packageId</span><span class="sxs-lookup"><span data-stu-id="5cb05-113">packageId</span></span>|<span data-ttu-id="5cb05-114">String</span><span class="sxs-lookup"><span data-stu-id="5cb05-114">String</span></span>|<span data-ttu-id="5cb05-115">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="5cb05-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cb05-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5cb05-116">Relationships</span></span>
<span data-ttu-id="5cb05-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5cb05-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5cb05-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cb05-118">JSON Representation</span></span>
<span data-ttu-id="5cb05-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cb05-119">Here is a JSON representation of the resource.</span></span>
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





