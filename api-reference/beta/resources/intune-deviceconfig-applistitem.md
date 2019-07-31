---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f985994ae3d69280ac1bd55626096cf6de46adf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971118"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="888dc-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="888dc-103">appListItem resource type</span></span>

> <span data-ttu-id="888dc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="888dc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="888dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="888dc-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="888dc-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="888dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="888dc-107">Properties</span></span>
|<span data-ttu-id="888dc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="888dc-108">Property</span></span>|<span data-ttu-id="888dc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="888dc-109">Type</span></span>|<span data-ttu-id="888dc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="888dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="888dc-111">name</span><span class="sxs-lookup"><span data-stu-id="888dc-111">name</span></span>|<span data-ttu-id="888dc-112">Строка</span><span class="sxs-lookup"><span data-stu-id="888dc-112">String</span></span>|<span data-ttu-id="888dc-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="888dc-113">The application name</span></span>|
|<span data-ttu-id="888dc-114">publisher</span><span class="sxs-lookup"><span data-stu-id="888dc-114">publisher</span></span>|<span data-ttu-id="888dc-115">String</span><span class="sxs-lookup"><span data-stu-id="888dc-115">String</span></span>|<span data-ttu-id="888dc-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="888dc-116">The publisher of the application</span></span>|
|<span data-ttu-id="888dc-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="888dc-117">appStoreUrl</span></span>|<span data-ttu-id="888dc-118">String</span><span class="sxs-lookup"><span data-stu-id="888dc-118">String</span></span>|<span data-ttu-id="888dc-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="888dc-119">The Store URL of the application</span></span>|
|<span data-ttu-id="888dc-120">appId</span><span class="sxs-lookup"><span data-stu-id="888dc-120">appId</span></span>|<span data-ttu-id="888dc-121">String</span><span class="sxs-lookup"><span data-stu-id="888dc-121">String</span></span>|<span data-ttu-id="888dc-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="888dc-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="888dc-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="888dc-123">Relationships</span></span>
<span data-ttu-id="888dc-124">Нет</span><span class="sxs-lookup"><span data-stu-id="888dc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="888dc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="888dc-125">JSON Representation</span></span>
<span data-ttu-id="888dc-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="888dc-126">Here is a JSON representation of the resource.</span></span>
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





