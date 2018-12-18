---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
ms.openlocfilehash: a7e33b986f95f610abff2c7b5321f48f3668e488
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323599"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="a44db-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="a44db-103">appListItem resource type</span></span>

> <span data-ttu-id="a44db-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a44db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a44db-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="a44db-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="a44db-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a44db-106">Properties</span></span>
|<span data-ttu-id="a44db-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a44db-107">Property</span></span>|<span data-ttu-id="a44db-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a44db-108">Type</span></span>|<span data-ttu-id="a44db-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a44db-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a44db-110">name</span><span class="sxs-lookup"><span data-stu-id="a44db-110">name</span></span>|<span data-ttu-id="a44db-111">String</span><span class="sxs-lookup"><span data-stu-id="a44db-111">String</span></span>|<span data-ttu-id="a44db-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="a44db-112">The application name</span></span>|
|<span data-ttu-id="a44db-113">publisher</span><span class="sxs-lookup"><span data-stu-id="a44db-113">publisher</span></span>|<span data-ttu-id="a44db-114">String</span><span class="sxs-lookup"><span data-stu-id="a44db-114">String</span></span>|<span data-ttu-id="a44db-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="a44db-115">The publisher of the application</span></span>|
|<span data-ttu-id="a44db-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a44db-116">appStoreUrl</span></span>|<span data-ttu-id="a44db-117">String</span><span class="sxs-lookup"><span data-stu-id="a44db-117">String</span></span>|<span data-ttu-id="a44db-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="a44db-118">The Store URL of the application</span></span>|
|<span data-ttu-id="a44db-119">appId</span><span class="sxs-lookup"><span data-stu-id="a44db-119">appId</span></span>|<span data-ttu-id="a44db-120">String</span><span class="sxs-lookup"><span data-stu-id="a44db-120">String</span></span>|<span data-ttu-id="a44db-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="a44db-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="a44db-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a44db-122">Relationships</span></span>
<span data-ttu-id="a44db-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a44db-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a44db-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a44db-124">JSON Representation</span></span>
<span data-ttu-id="a44db-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a44db-125">Here is a JSON representation of the resource.</span></span>
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



