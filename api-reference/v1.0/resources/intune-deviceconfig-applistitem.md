---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b9d7df95ce8ddb71439763eb02b205772e06300
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820323"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="62872-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="62872-103">appListItem resource type</span></span>

> <span data-ttu-id="62872-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62872-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62872-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="62872-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="62872-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62872-106">Properties</span></span>
|<span data-ttu-id="62872-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62872-107">Property</span></span>|<span data-ttu-id="62872-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62872-108">Type</span></span>|<span data-ttu-id="62872-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62872-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62872-110">name</span><span class="sxs-lookup"><span data-stu-id="62872-110">name</span></span>|<span data-ttu-id="62872-111">String</span><span class="sxs-lookup"><span data-stu-id="62872-111">String</span></span>|<span data-ttu-id="62872-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="62872-112">The application name</span></span>|
|<span data-ttu-id="62872-113">publisher</span><span class="sxs-lookup"><span data-stu-id="62872-113">publisher</span></span>|<span data-ttu-id="62872-114">String</span><span class="sxs-lookup"><span data-stu-id="62872-114">String</span></span>|<span data-ttu-id="62872-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="62872-115">The publisher of the application</span></span>|
|<span data-ttu-id="62872-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="62872-116">appStoreUrl</span></span>|<span data-ttu-id="62872-117">String</span><span class="sxs-lookup"><span data-stu-id="62872-117">String</span></span>|<span data-ttu-id="62872-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="62872-118">The Store URL of the application</span></span>|
|<span data-ttu-id="62872-119">appId</span><span class="sxs-lookup"><span data-stu-id="62872-119">appId</span></span>|<span data-ttu-id="62872-120">String</span><span class="sxs-lookup"><span data-stu-id="62872-120">String</span></span>|<span data-ttu-id="62872-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="62872-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="62872-122">Связи</span><span class="sxs-lookup"><span data-stu-id="62872-122">Relationships</span></span>
<span data-ttu-id="62872-123">Нет</span><span class="sxs-lookup"><span data-stu-id="62872-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62872-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62872-124">JSON Representation</span></span>
<span data-ttu-id="62872-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62872-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



