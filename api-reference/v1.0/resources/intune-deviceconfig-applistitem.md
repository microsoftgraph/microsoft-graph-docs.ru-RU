---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b9aa0a35767078b7c91f72b7a8b06a450cc9f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028611"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="cca79-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="cca79-103">appListItem resource type</span></span>

> <span data-ttu-id="cca79-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cca79-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cca79-105">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="cca79-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="cca79-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cca79-106">Properties</span></span>
|<span data-ttu-id="cca79-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cca79-107">Property</span></span>|<span data-ttu-id="cca79-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cca79-108">Type</span></span>|<span data-ttu-id="cca79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cca79-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cca79-110">name</span><span class="sxs-lookup"><span data-stu-id="cca79-110">name</span></span>|<span data-ttu-id="cca79-111">Строка</span><span class="sxs-lookup"><span data-stu-id="cca79-111">String</span></span>|<span data-ttu-id="cca79-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="cca79-112">The application name</span></span>|
|<span data-ttu-id="cca79-113">publisher</span><span class="sxs-lookup"><span data-stu-id="cca79-113">publisher</span></span>|<span data-ttu-id="cca79-114">String</span><span class="sxs-lookup"><span data-stu-id="cca79-114">String</span></span>|<span data-ttu-id="cca79-115">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="cca79-115">The publisher of the application</span></span>|
|<span data-ttu-id="cca79-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cca79-116">appStoreUrl</span></span>|<span data-ttu-id="cca79-117">String</span><span class="sxs-lookup"><span data-stu-id="cca79-117">String</span></span>|<span data-ttu-id="cca79-118">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="cca79-118">The Store URL of the application</span></span>|
|<span data-ttu-id="cca79-119">appId</span><span class="sxs-lookup"><span data-stu-id="cca79-119">appId</span></span>|<span data-ttu-id="cca79-120">String</span><span class="sxs-lookup"><span data-stu-id="cca79-120">String</span></span>|<span data-ttu-id="cca79-121">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="cca79-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="cca79-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="cca79-122">Relationships</span></span>
<span data-ttu-id="cca79-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cca79-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cca79-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cca79-124">JSON Representation</span></span>
<span data-ttu-id="cca79-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cca79-125">Here is a JSON representation of the resource.</span></span>
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



