---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253080"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="70c17-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="70c17-103">appListItem resource type</span></span>

> <span data-ttu-id="70c17-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70c17-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c17-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="70c17-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="70c17-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="70c17-106">Properties</span></span>
|<span data-ttu-id="70c17-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="70c17-107">Property</span></span>|<span data-ttu-id="70c17-108">Тип</span><span class="sxs-lookup"><span data-stu-id="70c17-108">Type</span></span>|<span data-ttu-id="70c17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70c17-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c17-110">name</span><span class="sxs-lookup"><span data-stu-id="70c17-110">name</span></span>|<span data-ttu-id="70c17-111">String</span><span class="sxs-lookup"><span data-stu-id="70c17-111">String</span></span>|<span data-ttu-id="70c17-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="70c17-112">The application name</span></span>|
|<span data-ttu-id="70c17-113">publisher</span><span class="sxs-lookup"><span data-stu-id="70c17-113">publisher</span></span>|<span data-ttu-id="70c17-114">String</span><span class="sxs-lookup"><span data-stu-id="70c17-114">String</span></span>|<span data-ttu-id="70c17-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="70c17-115">The publisher of the application</span></span>|
|<span data-ttu-id="70c17-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="70c17-116">appStoreUrl</span></span>|<span data-ttu-id="70c17-117">String</span><span class="sxs-lookup"><span data-stu-id="70c17-117">String</span></span>|<span data-ttu-id="70c17-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="70c17-118">The Store URL of the application</span></span>|
|<span data-ttu-id="70c17-119">appId</span><span class="sxs-lookup"><span data-stu-id="70c17-119">appId</span></span>|<span data-ttu-id="70c17-120">String</span><span class="sxs-lookup"><span data-stu-id="70c17-120">String</span></span>|<span data-ttu-id="70c17-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="70c17-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="70c17-122">Связи</span><span class="sxs-lookup"><span data-stu-id="70c17-122">Relationships</span></span>
<span data-ttu-id="70c17-123">Нет</span><span class="sxs-lookup"><span data-stu-id="70c17-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70c17-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70c17-124">JSON Representation</span></span>
<span data-ttu-id="70c17-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70c17-125">Here is a JSON representation of the resource.</span></span>
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



