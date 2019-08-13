---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 523944b68f899c770569c7e10fea539de2788f7a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333914"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="3980f-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="3980f-103">appListItem resource type</span></span>

> <span data-ttu-id="3980f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3980f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3980f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3980f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3980f-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="3980f-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="3980f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3980f-107">Properties</span></span>
|<span data-ttu-id="3980f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3980f-108">Property</span></span>|<span data-ttu-id="3980f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3980f-109">Type</span></span>|<span data-ttu-id="3980f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3980f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3980f-111">name</span><span class="sxs-lookup"><span data-stu-id="3980f-111">name</span></span>|<span data-ttu-id="3980f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="3980f-112">String</span></span>|<span data-ttu-id="3980f-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="3980f-113">The application name</span></span>|
|<span data-ttu-id="3980f-114">publisher</span><span class="sxs-lookup"><span data-stu-id="3980f-114">publisher</span></span>|<span data-ttu-id="3980f-115">String</span><span class="sxs-lookup"><span data-stu-id="3980f-115">String</span></span>|<span data-ttu-id="3980f-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="3980f-116">The publisher of the application</span></span>|
|<span data-ttu-id="3980f-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3980f-117">appStoreUrl</span></span>|<span data-ttu-id="3980f-118">String</span><span class="sxs-lookup"><span data-stu-id="3980f-118">String</span></span>|<span data-ttu-id="3980f-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="3980f-119">The Store URL of the application</span></span>|
|<span data-ttu-id="3980f-120">appId</span><span class="sxs-lookup"><span data-stu-id="3980f-120">appId</span></span>|<span data-ttu-id="3980f-121">String</span><span class="sxs-lookup"><span data-stu-id="3980f-121">String</span></span>|<span data-ttu-id="3980f-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="3980f-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="3980f-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="3980f-123">Relationships</span></span>
<span data-ttu-id="3980f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="3980f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3980f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3980f-125">JSON Representation</span></span>
<span data-ttu-id="3980f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3980f-126">Here is a JSON representation of the resource.</span></span>
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



