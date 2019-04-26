---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575095"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="cf549-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="cf549-103">appListItem resource type</span></span>

> <span data-ttu-id="cf549-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf549-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf549-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="cf549-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="cf549-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf549-106">Properties</span></span>
|<span data-ttu-id="cf549-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf549-107">Property</span></span>|<span data-ttu-id="cf549-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cf549-108">Type</span></span>|<span data-ttu-id="cf549-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf549-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf549-110">name</span><span class="sxs-lookup"><span data-stu-id="cf549-110">name</span></span>|<span data-ttu-id="cf549-111">String</span><span class="sxs-lookup"><span data-stu-id="cf549-111">String</span></span>|<span data-ttu-id="cf549-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="cf549-112">The application name</span></span>|
|<span data-ttu-id="cf549-113">publisher</span><span class="sxs-lookup"><span data-stu-id="cf549-113">publisher</span></span>|<span data-ttu-id="cf549-114">String</span><span class="sxs-lookup"><span data-stu-id="cf549-114">String</span></span>|<span data-ttu-id="cf549-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="cf549-115">The publisher of the application</span></span>|
|<span data-ttu-id="cf549-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cf549-116">appStoreUrl</span></span>|<span data-ttu-id="cf549-117">String</span><span class="sxs-lookup"><span data-stu-id="cf549-117">String</span></span>|<span data-ttu-id="cf549-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="cf549-118">The Store URL of the application</span></span>|
|<span data-ttu-id="cf549-119">appId</span><span class="sxs-lookup"><span data-stu-id="cf549-119">appId</span></span>|<span data-ttu-id="cf549-120">String</span><span class="sxs-lookup"><span data-stu-id="cf549-120">String</span></span>|<span data-ttu-id="cf549-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="cf549-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf549-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="cf549-122">Relationships</span></span>
<span data-ttu-id="cf549-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cf549-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf549-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf549-124">JSON Representation</span></span>
<span data-ttu-id="cf549-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf549-125">Here is a JSON representation of the resource.</span></span>
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



