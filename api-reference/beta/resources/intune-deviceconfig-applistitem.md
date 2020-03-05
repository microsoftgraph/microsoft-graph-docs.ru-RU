---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb861ad99aa3d8d73fd096af33377722c74feace
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527093"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="9046d-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="9046d-103">appListItem resource type</span></span>

<span data-ttu-id="9046d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9046d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9046d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9046d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9046d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9046d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9046d-107">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="9046d-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="9046d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9046d-108">Properties</span></span>
|<span data-ttu-id="9046d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9046d-109">Property</span></span>|<span data-ttu-id="9046d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9046d-110">Type</span></span>|<span data-ttu-id="9046d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9046d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9046d-112">name</span><span class="sxs-lookup"><span data-stu-id="9046d-112">name</span></span>|<span data-ttu-id="9046d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9046d-113">String</span></span>|<span data-ttu-id="9046d-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="9046d-114">The application name</span></span>|
|<span data-ttu-id="9046d-115">publisher</span><span class="sxs-lookup"><span data-stu-id="9046d-115">publisher</span></span>|<span data-ttu-id="9046d-116">String</span><span class="sxs-lookup"><span data-stu-id="9046d-116">String</span></span>|<span data-ttu-id="9046d-117">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="9046d-117">The publisher of the application</span></span>|
|<span data-ttu-id="9046d-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9046d-118">appStoreUrl</span></span>|<span data-ttu-id="9046d-119">String</span><span class="sxs-lookup"><span data-stu-id="9046d-119">String</span></span>|<span data-ttu-id="9046d-120">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="9046d-120">The Store URL of the application</span></span>|
|<span data-ttu-id="9046d-121">appId</span><span class="sxs-lookup"><span data-stu-id="9046d-121">appId</span></span>|<span data-ttu-id="9046d-122">String</span><span class="sxs-lookup"><span data-stu-id="9046d-122">String</span></span>|<span data-ttu-id="9046d-123">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="9046d-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9046d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9046d-124">Relationships</span></span>
<span data-ttu-id="9046d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9046d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9046d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9046d-126">JSON Representation</span></span>
<span data-ttu-id="9046d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9046d-127">Here is a JSON representation of the resource.</span></span>
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



