---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7e005681917f0edffe00b33947d2bd2bd5b2ff5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172249"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="ebfff-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="ebfff-103">appListItem resource type</span></span>

> <span data-ttu-id="ebfff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebfff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebfff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebfff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebfff-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="ebfff-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="ebfff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebfff-107">Properties</span></span>
|<span data-ttu-id="ebfff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebfff-108">Property</span></span>|<span data-ttu-id="ebfff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ebfff-109">Type</span></span>|<span data-ttu-id="ebfff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ebfff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebfff-111">name</span><span class="sxs-lookup"><span data-stu-id="ebfff-111">name</span></span>|<span data-ttu-id="ebfff-112">String</span><span class="sxs-lookup"><span data-stu-id="ebfff-112">String</span></span>|<span data-ttu-id="ebfff-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="ebfff-113">The application name</span></span>|
|<span data-ttu-id="ebfff-114">publisher</span><span class="sxs-lookup"><span data-stu-id="ebfff-114">publisher</span></span>|<span data-ttu-id="ebfff-115">String</span><span class="sxs-lookup"><span data-stu-id="ebfff-115">String</span></span>|<span data-ttu-id="ebfff-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="ebfff-116">The publisher of the application</span></span>|
|<span data-ttu-id="ebfff-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ebfff-117">appStoreUrl</span></span>|<span data-ttu-id="ebfff-118">String</span><span class="sxs-lookup"><span data-stu-id="ebfff-118">String</span></span>|<span data-ttu-id="ebfff-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="ebfff-119">The Store URL of the application</span></span>|
|<span data-ttu-id="ebfff-120">appId</span><span class="sxs-lookup"><span data-stu-id="ebfff-120">appId</span></span>|<span data-ttu-id="ebfff-121">String</span><span class="sxs-lookup"><span data-stu-id="ebfff-121">String</span></span>|<span data-ttu-id="ebfff-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="ebfff-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebfff-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ebfff-123">Relationships</span></span>
<span data-ttu-id="ebfff-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ebfff-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebfff-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebfff-125">JSON Representation</span></span>
<span data-ttu-id="ebfff-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebfff-126">Here is a JSON representation of the resource.</span></span>
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




