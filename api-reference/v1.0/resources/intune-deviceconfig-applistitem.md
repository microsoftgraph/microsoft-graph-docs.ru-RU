---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c43b559f1c1994d34ae0d4202b4970227d029df7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366743"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="42111-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="42111-103">appListItem resource type</span></span>

> <span data-ttu-id="42111-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42111-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42111-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="42111-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="42111-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="42111-106">Properties</span></span>
|<span data-ttu-id="42111-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="42111-107">Property</span></span>|<span data-ttu-id="42111-108">Тип</span><span class="sxs-lookup"><span data-stu-id="42111-108">Type</span></span>|<span data-ttu-id="42111-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42111-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42111-110">name</span><span class="sxs-lookup"><span data-stu-id="42111-110">name</span></span>|<span data-ttu-id="42111-111">Строка</span><span class="sxs-lookup"><span data-stu-id="42111-111">String</span></span>|<span data-ttu-id="42111-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="42111-112">The application name</span></span>|
|<span data-ttu-id="42111-113">publisher</span><span class="sxs-lookup"><span data-stu-id="42111-113">publisher</span></span>|<span data-ttu-id="42111-114">String</span><span class="sxs-lookup"><span data-stu-id="42111-114">String</span></span>|<span data-ttu-id="42111-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="42111-115">The publisher of the application</span></span>|
|<span data-ttu-id="42111-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="42111-116">appStoreUrl</span></span>|<span data-ttu-id="42111-117">String</span><span class="sxs-lookup"><span data-stu-id="42111-117">String</span></span>|<span data-ttu-id="42111-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="42111-118">The Store URL of the application</span></span>|
|<span data-ttu-id="42111-119">appId</span><span class="sxs-lookup"><span data-stu-id="42111-119">appId</span></span>|<span data-ttu-id="42111-120">String</span><span class="sxs-lookup"><span data-stu-id="42111-120">String</span></span>|<span data-ttu-id="42111-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="42111-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="42111-122">Связи</span><span class="sxs-lookup"><span data-stu-id="42111-122">Relationships</span></span>
<span data-ttu-id="42111-123">Нет</span><span class="sxs-lookup"><span data-stu-id="42111-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42111-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42111-124">JSON Representation</span></span>
<span data-ttu-id="42111-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42111-125">Here is a JSON representation of the resource.</span></span>
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




